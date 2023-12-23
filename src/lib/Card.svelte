<script>
    export let title, content

    export let cardClasses; //tailwind classes for card element

</script>



<div id="card" class={cardClasses}>
    <h2 class="font-bold text-gray-700">{title}</h2>
    <p class="mt-5 text-gray-500">{content}</p>
</div>




<style>
    #card {
        background-color: rgba(128, 128, 128, 0.058);
    }
</style>