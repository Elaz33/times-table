
<script lang="ts">
   
    let numRows = 10;
    let numCols =   10;
    let incrementor  = 0;
     const rows:number[] =[...Array(numRows)];
     const rowItems:number[]= [...Array(numCols)]
     
</script>
<h1 class="header">Times Table</h1>
{#each rowItems as rowItem}
    <input type="number" bind:value ={rowItem}/>
{/each}
<div class="outer-box">
    {#each  rows  as row,i}
    <div class="row">
        {#each rowItems as rowItem,i}
            <div class="row-item"contenteditable ="true" bind:textContent={rowItem}>{i}</div>
        {/each}
    </div>
      {/each}
</div>

<style>
    .header{
        text-align: center;
    }
    .row{
        display: flex;
        border: solid black;
    }
    .row-item{
        border: solid black;
        flex: 1;
        text-align: center;
    }
</style>

