<script>
    import Layout from "../routes/+layout.svelte";

    export let y;

    let tabs = [
        { name: "About me", link: "#about" },
        { name: "Projects", link: "#projects" },
        { name: "Education", link: "#Education" },
        { name: "Skills", link: "#Skills" },
    ];
</script>

<header
    class={"sticky z-[20] top-0 duration-200 px-6 flex items-center justify-between border border-solid" +
        (y > 0
            ? " py-4 bg-black border-red-700"
            : " py-6 bg-transparent border-transparent")}
>
    <a href="#" class="hover:text-slate-950">
        <h1 class="font-medium">
            <b class="font-bold ubuntu">Franz</b> Leeann Ferry
        </h1>
    </a>
    <div class="sm:flex ml-auto pr-4 items-center gap-4 hidden ">
        {#each tabs as tab, index}
            <a href={tab.link} class="duration-200 hover:text-red-450 hover:text-slate-950">
                <p>{tab.name}</p>
            </a>
        {/each}
    </div>
    <a
        href="https://mail.google.com/mail/?view=cm&fs=1&to=fluferry@mymail.mapua.edu.ph"
        target="_blank"
        class="blueShadow relative overflow-hidden px-5 py-2 group rounded-full bg-white text-slate-950 hover:bg-gray-200"
    >
        <div
            class="absolute top-0 right-full w-full h-full bg-red-950 opacity-20 group-hover:-translate-x-full z-0 duration-200"
        ></div>
        <h4 class="relative z-9">Get in Touch</h4>
    </a>
</header>
