<script>
    import Step from "./Step.svelte";

    let steps = [
        {name: ' Charme Salon & Spa Website ', icon: ' fa-solid fa-table '},
        {name: ' CanvasHub ', icon: ' fa-solid fa-cart-shopping '},
        {name: ' Dog Adoption Mobile Application ', icon: ' fa-solid fa-dog '},
    ]
</script>

<main class="flex flex-col flex-1 p-4">
    <section
        id="introPage"
        class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
    >
        <div
            class="flex flex-col lg:justify-center text-center lg:text-justify gap-6 md:gap-5 lg:gap-10"
        >
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                Greetings! I'm <span class="unbuntu text-red-200"
                    >Franz Leeann Ferry</span
                > <br />Front-End
                <span class="unbuntu text-red-200">Developer</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
                I'm a <span class="unbuntu text-red-200"
                    >front-end developer</span
                >
                with a passion for creating Reactive, Functional and functional websites.
                I'm currently working on my
                <span class="unbuntu text-red-200">skills</span>
                in
                <span class="unbuntu text-red-200"
                    >Svelte, Tailwind CSS, OutSystems and other technologies</span
                >. I'm also working towards the
                <span class="unbuntu text-red-200">Game Development</span> Track
                to create Functional and Dynamic, Interesting games
            </p>
            <a
                class="blueShadow mx-auto lg:mr-auto text-base sm:text-lg md:text-xl ubuntu
                relative overflow-hidden px-5 py-2 group rounded-full hover:bg-gray-200 bg-white text-slate-950
                cursor-pointer"
                href="https://mail.google.com/mail/?view=cm&fs=1&to=fluferry@mymail.mapua.edu.ph"
                target="_blank"
            >
                <div
                    class="absolute top-0 right-full h-full bg-red-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
                />
                <h4 class="relative z-9">Get in Touch &rarr;</h4>
            </a>
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <img
                src={"images/profile.png"}
                alt="Profile"
                class="object-cover z-[2] max-h-[70vh]"
            />
        </div>
    </section>
    <section
        id="about"
        class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
    >
        <div
            class="flex flex-col lg:justify-center text-justify lg:text-justify gap-6 md:gap-5 lg:gap-10"
        >
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                <span class="ubuntu text-red-200">About</span> Me
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
                My Name is Franz Leeann U. Ferry, a College Student under the
                Computer Science course in Mapua University. I strive to become
                a successful Game Developer in the near future. At a very you
                age I was very passionate towards playing video games and I
                dreamt to create my very own when I grow up. I've also became
                interested in Web Development and I'm currently learning it. I
                wanted to create dynamic and reactive websites and as i was
                learning about Web Development, I found it engaging and really
                interesting and now I do everything I can to achieve that dream
                and be able to create, inovate and create websites and video
                games that really engages each and every one of us. This
                portfolio serves as a collection of my Academic Progress.
            </p>
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <img
                src={"images/me.jpg"}
                alt="Just Me"
                class="object-cover z-[10] max-h-[70vh]"
            />
        </div>
    </section>
    <section id="projects" class="py-20 lg:py-32 flex flex-col gap-24">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-lg sm:text-xl md:text-2xl">
                <span class="unbuntu text-red-200"
                    >Few Projects That I've created:</span
                >
            </h6>
            <h3 class="font-semibold text-3lg sm:text-4xl md:text-5xl">
                Curious to see my Work? <span class="unbuntu text-red-300"
                    >Check them out!</span
                >
            </h3><br><br>
            <div class="relative shadow-2xl grid place-items-Left">
                <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-18">
                    <Step step={steps [0]}>
                        <p>The Charme Salon & Spa Website is a freelance project and serves as a first project created by my group <strong class="text-red-400">Webguild. </strong>
                        It is created using <strong class="text-red-400">REACT, PHP Laravel, HTML and CSS.</strong> My role in the project is the <strong class="text-red-400">Front-end developer</strong>
                    and <strong class="text-red-400">UI/UX Designer</strong></p>
                    </Step>
                    <Step step={steps [1]}>
                        <p>The CanvasHub A full pledge mobile application that gives consumers an option of different prices across multiple stores of the same product.
                            This is developed using <strong class="text-red-400">Android Studios </strong>and <strong class="text-red-400">Springboot.</strong>
                        My role in the project is the <strong class="text-red-400">Front-end Developer</strong> and <strong class="text-red-400">UI/UX Designer</strong></p>
                    </Step>
                    <Step step={steps [2]}>
                        <p>The Dog Adoption Mobile Application is a mobile app that lets users browse, look and adopt dogs. This was developed using <strong class="text-red-400">
                            Android Studios</strong> and <strong class="text-red-400">IntelliJ also using Springboot.</strong></p>
                    </Step>
                </div>
            </div>
        </div>
    </section>
    <section
        id="Education"
        class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
    >

    </section>
    <section
    id="Skills"
    class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
>

</section>
</main>
