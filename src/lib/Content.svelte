<script>
    import Card from "./Card.svelte";
    import CardData from './CardData.json'
</script>


<section class="pt-10">

    {#each CardData as data (data.id)}
    
        <Card title={data.title} content={data.content}/>

    {/each}

    

</section>


<style>

</style>