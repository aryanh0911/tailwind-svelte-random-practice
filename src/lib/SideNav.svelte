<script>

    let closeSideNav = ()=>{
        document.getElementById('side-nav').classList.add("hidden")
        document.getElementById('sideNavWrapper').classList.add("hidden")
    }

    
</script>

    <section id="sideNavWrapper" class="hidden" on:click|self={closeSideNav}>
        <div id="side-nav" class="hidden fixed top-0 bottom-0 h-full right-0 w-2/3 bg-gray-200 shadow-xl">
    
            <button id="close-side-nav" on:click={closeSideNav} class="absolute right-8 top-5">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" data-slot="icon" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                  </svg>
                  
            </button>
        
            <div class="menuOptions flex flex-col gap-10 mt-20">
                <p class="inline-block font-bold pl-5">About</p>
                <p class="inline-block font-bold pl-5">Projects</p>
                <p class="inline-block font-bold pl-5">Contact</p>
            </div>
        
        
        </div>
    </section>




<style>

    #sideNavWrapper {
        position: fixed;
        background-color: rgba(0,0,0,0.6);
        position: absolute;
        top: 0;
        bottom: 0;
        width: 100vw;
        height: 125vh;
        backdrop-filter: blur(2px);
    }
</style>