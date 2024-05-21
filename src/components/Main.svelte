<script lang="ts" >
    

    let benefits = [
        {
            metric: "10x",
            name: "a self taught developer",
            description:
                " While I studied Petroleum Engineering, my real passion was always software engineering. So, I started leveraging online resources and embarked on a self-taught journey. I loved the creativity and problem-solving that come with building innovative online experiences. I began with JavaScript, HTML, and CSS, and then dove into JavaScript frameworks and eventually into backend programming and design principles. This ongoing learning keeps me excited about the ever-evolving world of web development.",
        },
        {
            name: "a Pixel Perfect Fanatic",
            description:
                "Crafting pixel-perfect designs with great user experiences lets me express and experiment with my creativity. I love the challenge of learning new design concepts and creating amazing online experiences for users. I strive to bring the product designer's vision to life by ensuring a pixel perfect replication of the design and a seamless user experience.",
        },
        {
            name: "an excellent communicator",
            description:
                "Communication is key and it's a paramount value of mine. I believe in transparency and constructive communication above all else. This helps me develop deep relationships and ensures my effectiveness and productivity in any work space with any team.",
        },
    ];
</script>

<main class="flex flex-col flex-1 p-4">
    <section
        id="introPage"
        class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
    >
        <div
            class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10"
        >
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hi! I'm <span class="poppins text-green-400">Olalekan</span> Abdulfatah
                <br />Frontend
                <span class="poppins text-green-400">Engineer</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl"> Senior Frontend developer <span class="text-green-400"> | </span> Happiness Connoisseur  </p>
            <p> Svelte <span class="text-green-400"> | </span> React <span class="text-green-400"> | </span> Next <span class="text-green-400"> | </span> Vue<span class="text-green-400"> | </span> </p>
            <button
                class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950"
            >
                <div
                    class="absolute top-0 right-full w-full h-full bg-green-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
                />
                <a href="https://blog.lekan.dev/" target="_blank" class="relative z-9">Visit Blog &rarr;</a>
            </button>
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <img
                src={"images/profile.png"}
                alt="Zetane Engine"
                class="object-cover z-[2] max-h-[70vh]"
            />
        </div>
    </section>
    
    <section
        id="about"
        class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
    >
        <!-- <div class="z-[-1] bg-green-950 w-screen left-1/2 -translate-x-1/2 top-0 h-full absolute"> </div> -->
        <div
            class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-green-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-green-700 py-4"
        >
            
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                A bit more <span class="poppins text-green-400">about</span> me.
            </h3>

            <h6 class="text-large sm:text-xl md:text-2xl">
                I am ...
            </h6>
        </div>
        <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
            {#each benefits as benefit, index}
                <div class="flex gap-6 sm:gap-8">
                    <p
                        class="poppins text-4xl sm:text-5xl md:text-6xl text-green-400 font-semibold"
                    >
                        0{index + 1}
                    </p>
                    <div class="flex flex-col gap-6 sm:gap-8">
                        <h3 class="text-2xl sm:text-3xl md:text-5xl">
                            {benefit.name}
                        </h3>
                        <p>{benefit.description}</p>
                    </div>
                </div>
            {/each}
        </div>
    </section>
</main>
