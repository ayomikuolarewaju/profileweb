<script>
	import Head from '$lib/components/Head.svelte';
    import "../app.css";
  import Footer from '$lib/components/Footer.svelte';

  let y = 0;
  let innerHeight = 0
  let innerWidth = 0
  const gotop =()=>{
    document.body.scrollIntoView()
  }
  </script>

  <div class="relative flex flex-col max-w-[1400px] mx-auto w-full text-sm sm:text-base min-h-screen">

    <div class={"fixed bottom-0 w-full duration-200 p-10 z-[-10] flex "  + (y > 0 ? 'opacity-full pointer-events-auto' : 'opacity-0 pointer-events-none')}>
      <button  on:click={gotop} class="mt-auto rounded-full aspect-square bg-slate-900 text-violet-400 px-3 
      sm:px-4 cursor-auto hover:bg-slate-400 z-1">
        <i class="fa-solid fa-arrow-up grid place-items-center aspect-square"/></button>
    </div>

    <Head {y}/>
    
    <slot />
    <Footer/>
  </div>

  <svelte:window bind:scrollY={y} bind:innerHeight bind:innerWidth/>
  
