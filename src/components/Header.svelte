<script>
    export let y;
    let tabs=[
        {name: 'Projects',link: '#projects'},
        {name: 'About Me',link: '#about'},
        
    ]
</script>

<header class={'sticky z-[10] top-0 duration-200 px-6 flex items-center justify-between border border-solid ' + (y>0 ? ' py-4 bg-slate-950 border-blue-950' : ' py-6 bg-transparent border-transparent')}>
<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-J560TP1V7H"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'G-J560TP1V7H');
</script>
<!-- Google tag (gtag.js) -->
    <h1>
        <b class="font-bold poppins">Juan</b> Rodriguez
    </h1>

    <div class="sm:flex ml-auto pr-4 items-center gap-4 hidden">
        {#each tabs as tab, index }
            <a href={tab.link} class="duration-200 hover:text-blue-400"> <!--Change color of links hover-->
                <p>
                    {tab.name}
                </p>
            </a>
        {/each}
    </div>
    <a href="https://www.linkedin.com/in/juan-rodriguez-26b39427a/" target="_blank" class="blueShadow relative overflow-hidden px-5 py-2 group rounded-full bg-white text-slate-950">
        <div class="absolute top-0 right-full w-full h-full bg-blue-400 opacity-20 group-hover:translate-x-full z-0 duration-200">
        </div>
        <h4 class="relative z-9">Get in touch!</h4>
    </a>
</header>
