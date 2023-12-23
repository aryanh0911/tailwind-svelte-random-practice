<script>

        import { gsap } from "gsap";
        import { ScrollTrigger } from "gsap/ScrollTrigger";
        gsap.registerPlugin(ScrollTrigger);
        import { onMount } from "svelte"


    let openSideNav = ()=>{
        if(document.querySelector('#side-nav').classList.contains("hidden")){
            document.querySelector('#side-nav').classList.remove("hidden")
        }
       
        if(document.querySelector('#sideNavWrapper').classList.contains("hidden")){
            document.querySelector('#sideNavWrapper').classList.remove("hidden")
        }

    }


// GSAP ANIMATIONS
    onMount(()=>{

        var tl = gsap.timeline()

        tl.from("#logo",{
            y:"-10",
            opacity: 0,
        })
    });

</script>


<header class="fixed w-full p-12 pb-9 flex justify-between shadow-lg">
    <a href="" id="logo" class="logo-crimson"> Logo </a>

    <nav class="flex gap-7 text-xl ">

        <a href="" class="hidden md:block">About</a>
        <a href="" class="hidden md:block">Projects</a>
        <a href="" class="hidden md:block">Contact</a>

        <button id="hamburger-btn" on:click={openSideNav}>
            <svg class="w-6 h-6 md:hidden" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" data-slot="icon" >
                <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
                </svg>
        </button>
    </nav>
</header>


<style>
    header {
        /* position: fixed; */
        /* z-index: 99; */
        background-color: #ffffff38;
        backdrop-filter: blur(10px);
    }

    #logo {
        transition: text-shadow .3s;
    }

    #logo:hover {
        text-shadow: 4px 4px 3px rgba(0, 255, 255, 0.719);
    }
</style>