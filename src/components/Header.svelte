<script>
    
    import Logo from "./Logo.svelte";
    export let y;

    export let tabs = [
        { name: "About me", link: "#about" },
        { name: "Contact", link: "#contact" },
    ];
</script>

<header
    class={"sticky z-[10] top-0 duration-200 px-6 flex items-center justify-between border-b border-solid " +
        (y > 0
            ? " py-4 bg-slate-950 border-green-950"
            : " py-6 bg-transparent border-transparent")}
>
    <h1 class="font-medium">
        <!-- <b class="font-bold poppins">Olalekan</b> <span class="">Abdulfatah</span> -->
        <Logo />
    </h1>
    <div class="sm:flex items-center gap-4 hidden">
        {#each tabs as tab, index}
            <a
                href={tab.link}
                class="duration-200 hover:text-green-400"
                target={index === 2 ? "_blank" : ""}
            >
                <p>{tab.name}</p>
            </a>
        {/each}
      
        <a
        target="_blank"
        href="https://blog.lekan.dev"
            class="blueShadow relative overflow-hidden px-5 py-2 group rounded-full bg-white text-slate-950"
        >
            <div
                class="absolute top-0 right-full w-full h-full bg-green-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
            />
            <h4 class="relative z-9">Visit blog</h4>
        </a>
    </div>
</header>
