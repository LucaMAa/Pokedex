<script>
   import {pokemon} from '../Stores/PokeStore';
   import PokemanCard from '../Components/PokemanCard.svelte';

   let searchterm ="";
   let filterPokemon =[];

   $: {
       console.log(searchterm);
       if(searchterm)
       {
           //search the pokemon
           filterPokemon = $pokemon.filter(Pokeman=> Pokeman.name.toLowerCase().includes(searchterm.toLowerCase()));
       }else{
           filterPokemon = [... $pokemon]
       }
   }

</script>
<svelte:head>
    <title >Pokedex Head</title>
</svelte:head>
<body class="body1">
<a href="/">
    <img src="https://fontmeme.com/permalink/211007/ec6f1282637dc5e322271014f29baece.png" alt="font-pokemon" border="0">
</a>





<input class="w-full rounded-md text-lg p-4 border-2 border-gray-200" type="text" bind:value={searchterm} placeholder="Search Your Pokemon ✍">
<div class="py-4 grid gap-4 md:grid-cols-3 gird-cols-2">
    {#each filterPokemon as Pokeman }
   <PokemanCard pokeman={Pokeman}/>
{/each}</div> 
</body>

<style>

    .body1
    {
        background-image: url("../BackGround.jpg");
        background-size: cover;
    }
    
</style>



