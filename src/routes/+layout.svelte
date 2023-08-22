<script lang="ts">
     import Footer from "../components/Footer.svelte";
      import Header from "../components/Header.svelte";
      import "../app.css";
      export let y: number;
      $: y = 0;

      let innerWidth = 0;  //to be used
      let innerHeight:number;

      function goTop() {
          document.body.scrollIntoView();
      }

  </script>
  
  <div
  
  class="container relative flex flex-col max-w-[1400px] mx-auto w-full text-sm sm:text-base min-h-screen"
>
  <!-- TODO: scroll btn -->
  <Header {y} {innerHeight}/>
  <slot />
  <Footer />
</div>
<!-- TODO: Change to main -->