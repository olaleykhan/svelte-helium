<script lang="ts">
     import Footer from "../components/Footer.svelte";
      import Header from "../components/Header.svelte";
      import "../app.css";
      let y: number;

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

<svelte:window bind:scrollY={y} bind:innerHeight bind:innerWidth />