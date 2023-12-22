<script>

    let closeSideNav = ()=>{
        document.getElementById('side-nav').classList.add("hidden")
        document.getElementById('modalSection').classList.add("hidden")
    }

    
</script>

    <section id="modalSection" class="hidden" on:click|self={closeSideNav}>
        <div id="side-nav" class="hidden absolute h-screen top-0 right-0 w-2/3 bg-blue-100 shadow-xl">
    
            <button id="close-side-nav" on:click={closeSideNav} class="absolute right-2 top-2">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" data-slot="icon" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                  </svg>
                  
            </button>
        
            <div class="menuOptions flex flex-col gap-10 mt-20">
                <p class="inline-block font-bold pl-5">One</p>
                <p class="inline-block font-bold pl-5">Two</p>
                <p class="inline-block font-bold pl-5">Three</p>
            </div>
        
        
        </div>
    </section>




<style>
    /* #side-nav {
        display: block;
    }     */

    section {
        background-color: rgba(0,0,0,0.8);
        position: absolute;
        background-color: rgba(0,0,0,0.8);
        width: 100vw;
        height: 100vh;
        top: 0;
        backdrop-filter: blur(2px);
    }
</style>