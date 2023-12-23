<script>
    import Card from "./Card.svelte";
    import CardData from './CardData.json'



    let alterMargin = (id)=>{

        let cardClasses = "p-4 pb-16 max-w-lg rounded-lg mb-8 shadow-lg " //tailwind classes of Card element

        if(id%2 === 0){
           cardClasses += " ml-auto" //adds margin-left:auto
        }
        else{
            cardClasses += " mr-auto" //adds margin-right:auto
        }
        return cardClasses;
    }

</script>


<section class="bg-slate-200 pt-48 pb-6 px-8 md:px-20 lg:px-48 xl:px-56 2xl:px-96">
    
    {#each CardData as data, i}
    
        <Card title={data.title} content={data.content} cardClasses={alterMargin(i+1)} />

    {/each}

</section>



<style>

</style>