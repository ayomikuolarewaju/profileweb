<script>
    export let y;
    let tabs = [ { index:1,name:'Projects',link:'#projects'},
        { index:2,name:'About me',link:'#about'},]

</script>

<header class={"sticky z-[10] top-0 duration-200 px-4 flex items-center justify-between border border-solid " +
 ( y>0 ? 'py-4 bg-slate-950 border-slate-950' : 'py-6 bg-transparent border-transparent')}>
    <h1 class="font-medium" id="">
        <b class="font-bold poppins">Almaroof</b> Olarewaju</h1>

    <div class="sm:flex items-center gap-4 hidden ml-auto pr-4">
      {#each tabs as tab (tab.index)}

      <a href="{tab.link}" class="hover:text-violet-400 duration-200"><p>{tab.name}</p></a>
       
      {/each}
    </div>
    <a href="/" target="_blank" class="blueShadow rounded-full text-slate-950 bg-white w-[150px] hover:bg-slate-800 hover:text-white">
        <div>
         <h4 class="z-9 relative p-2 text-center">Get In Touch</h4>
        </div>
    </a>
</header>