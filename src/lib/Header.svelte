<script>

    let openSideNav = ()=>{
        if(document.querySelector('#side-nav').classList.contains("hidden")){
            document.querySelector('#side-nav').classList.remove("hidden")
        }

    }
</script>


<header class="p-12 pb-9 flex justify-between border border-b-gray-400 border-spacing-2">
    <a href="" class="logo-blue"> Logo </a>

    <nav class="flex gap-7 text-xl ">

        <a href="" class="hidden md:block">About</a>
        <a href="" class="hidden md:block">Projects</a>
        <a href="" class="hidden md:block">Know More</a>

        <button id="hamburger-btn" on:click={openSideNav}>
            <svg class="w-6 h-6 md:hidden" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" data-slot="icon" >
                <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
                </svg>
        </button>
    </nav>
</header>


<style>

</style>