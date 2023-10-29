<script>
	
	import Step from './Step.svelte';

    let step = [
        {name:'lekan stores',icon:'fa-solid fa-cart-shopping'},
        {name:'lekan stores',icon:'fa-solid fa-list-check'},
        {name:'lekan stores',icon:'fa-solid fa-diagram-project'}
    ]

    let benefits = [
        {name:'A Self Taught Developer',descripion:'Start by creating a new SvelteKit project if you don\'t have one set up already. The most common approach is outlined in the Getting Started with SvelteKit introduction.'},
        {name:'Execellent Team Player',descripion:'Start by creating a new SvelteKit project if you don\'t have one set up already. The most common approach is outlined in the Getting Started with SvelteKit introduction.'},
        {name:'Awesome Attention To Details',descripion:'Start by creating a new SvelteKit project if you don\'t have one set up already. The most common approach is outlined in the Getting Started with SvelteKit introduction.'}
    ]

</script>



<main class="flex flex-col flex-1 p4">
    <section id="into"  class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14">
        <div class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-14">
            <h2 class="font-bold text-4xl sm:text-5xl md:text-6xl">Hi! I'm <span class="poppins text-violet-400">Almaroof </span>Olarewaju <b/> Full Stack
            <span class="poppins text-violet-400">Developer</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl p-3">
                My <span class="text-violet-400">Favorite Tech</span> include Javascript, Svelte.js, Sveltekit, Tailwindcss, Node.js + express.jss , Mongodb + Mongoose & Flutter.
            </p>
            <a href="/" target="_blank" class="blueShadow rounded-full text-slate-950 bg-white w-[150px] hover:bg-slate-800 hover:text-white mx-auto">
                <div>
                 <h4 class="z-9 relative p-2 text-center">Get In Touch &rarr;</h4>
                </div>
            </a>

        </div>

        <div class="place-items-center relative grid shadow-2xl">
          <img src="images/profile.png" alt="profile pic" srcset="" class="object-cover z-[2] max-h-[70vh]">
        </div>

    </section>

    <section id="projects" class="py-20 lg:py-32 flex flex-col gap-10">
        <div class="flex flex-col gap-2 text-center">
            <h4 class="text-lg sm:text-xl md:text-2xl">A few of my Creations</h4>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">Curious to <span class="text-violet-400">see</span> my work?</h3>

        </div>
        <div class=" flex flex-col items-center text-center place-items-center">
            <a href="/" target="_blank" class="blueShadow rounded-full text-slate-950 bg-white aspect-square w-[50px] hover:bg-slate-800 hover:text-white  ">
                <i class="fa-regular fa-circle-play text-center"/>
            </a>
            
        </div>

           <div class="grid grid-cols-1 gap-12 lg:gap-12 p-5">
            <Step step = {step[0]}>
                <p>lekan stores is an E-commerce created with  
                <strong class="text-violet-400">Sveltekit,Svelte,Nodejs Expressjs Commercejs and Strip</strong>
                Commercejs is a product CMS while Strip is a payment gate way
                </p>
            </Step>
            <Step step = {step[1]}>
                <p>lekan stores is an E-commerce created with  
                    <strong class="text-violet-400">Sveltekit,Svelte,Nodejs Expressjs Commercejs and Strip</strong>
                    Commercejs is a product CMS while Strip is a payment gate way
                </p>
            </Step>
            <Step step = {step[2]}>
                <p>lekan stores is an E-commerce created with  
                    <strong class="text-violet-400">Sveltekit,Svelte,Nodejs Expressjs Commercejs and Strip</strong>
                    Commercejs is a product CMS while Strip is a payment gate way
                </p>
            </Step>
           </div>
    </section>
    <section id="about" class="py-20 pt-10 lg:py-16 lg:pt-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative">
        <div  class="flex flex-col relative gap-2 text-center before:absolute before:top-0 before:left-0 before:w-2/3
        before:h-1.5 before:bg-violet-400 after:absolute after:bottom-0 after:right-0 after:w-2/3
        after:h-1.5 after:bg-violet-400 py-4">

        <h4  class="text-lg sm:text-xl md:text-2xl">Want to know more?</h4>
        <h3 class="font-semibold text-3xl sm:text-3xl md:text-4xl">A bit <strong class="poppins text-violet-400">About</strong></h3>

        </div>

        <p class="mx-auto text-lg font-semibold poppins sm:text-xl md:text-2xl">I am . . .</p>
        <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px] pl-5">
            {#each benefits as benefit, index}
                <div class="flex gap-6 sm:gap-8">
                  <p class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold">0{index + 1}</p>
                  <div class="flex flex-col gap-6 sm:gap-8">
                    <h3 class="text-2xl sm:text-3xl md:text-5xl">{benefit.name}</h3>
                    <p>{benefit.descripion}</p>
                  </div>
                </div>
            {/each}

        </div>
       <h5 class="font-semibold poppins text-2xl sm:text-3xl text-center">The <span class="text-violet-400">Complete</span> Package</h5>
       <div class="flex flex-col overflow-x-scroll gap-10 max-w-[1000px] mx-auto w-full">
           <table class="bg-white text-slate-400 text-center rounded">
            <thead class="border-b border-solid border-slate-400">
             <tr>
                <th/>
                <th class="whitespace-nowrap p-2 px-4">Candidate #1</th>
                <th class="whitespace-nowrap p-2 px-4">Candidate #2</th>
                <th class="whitespace-nowrap p-2 px-4">Candidate #3</th>
                <th class="whitespace-nowrap p-2 px-4 bg-violet-700 text-white">Me</th>
             </tr>
            </thead>
            <tbody>
              <tr class="border-b border-solid border-slate-500">
                <td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm">Dedication</td>
                <td><i class="fa-solid fa-xmark text-slate-500"></td>
                <td><i class="fa-solid fa-xmark text-slate-500"></td> 
                <td><i class="fa-solid fa-xmark text-slate-500"></td>
                <td><i class="fa-solid fa-check text-green-500"></td>   
              </tr>
              <tr class="border-b border-solid border-slate-500">
                <td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm">Critical Thougth</td>
                <td><i class="fa-solid fa-xmark text-slate-500"></td>
                <td><i class="fa-solid fa-xmark text-slate-500"></td> 
                <td><i class="fa-solid fa-xmark text-slate-500"></td>
                <td><i class="fa-solid fa-check text-green-500"></td>   
              </tr>
              <tr class="border-b border-solid border-slate-500">
                <td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm">Interpersonal Skill</td>
                <td><i class="fa-solid fa-xmark text-slate-500"></td>
                <td><i class="fa-solid fa-xmark text-slate-500"></td> 
                <td><i class="fa-solid fa-xmark text-slate-500"></td>
                <td><i class="fa-solid fa-check text-green-500"></td>   
              </tr>
              <tr class=" border-solid border-slate-500">
                <td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm">Programming Ability</td>
                <td><i class="fa-solid fa-xmark text-slate-500"></td>
                <td><i class="fa-solid fa-xmark text-slate-500"></td> 
                <td><i class="fa-solid fa-xmark text-slate-500"></td>
                <td><i class="fa-solid fa-check text-green-500"></td>   
              </tr>
            </tbody>
           </table>
       </div>
       <div class="mx-auto -mt-12 sm:hidden  italic opacity-50">
        <p>Scroll to see more &rarr;</p>
       </div>
       <p class="mx-auto">Why not invest?</p>
    </section>
    <div  class="m-20 p-5 bg-slate-500 rounded-full aspect-square w-[50px] h-[50px] sticky text-center flex items-center justify-center">
        <a href="#into" class="text-3xl"><p>&UpArrowBar;</p></a>
        
    </div>
</main>