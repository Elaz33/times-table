<script lang="ts">
    import { each } from "svelte/internal";

    let numFirstTwoRows = 10;
    let numFirstTwoCols = 1;

    let Cols = 1;
    let Rows = 10;
    let incrementor = 0;

    const cols: number[] = [...Array(numFirstTwoCols)];
    const cols2: number[] = [...Array(Cols)];
    const cols3: number[] = [...Array(Cols)];
    const cols4: number[] = [...Array(Cols)];
    const cols5: number[] = [...Array(Cols)];
    const cols6: number[] = [...Array(Cols)];
    const cols7: number[] = [...Array(Cols)];
    const cols8: number[] = [...Array(Cols)];
    const cols9: number[] = [...Array(Cols)];
    const cols10: number[] = [...Array(Cols)];

    const rowItems: number[] = [...Array(numFirstTwoRows)].map(() => {
        return (incrementor += 1);
    });
    incrementor = 0;
    const rowItems2: number[] = [...Array(Rows)].map(() => {
        return (incrementor += 2);
    });
    incrementor = 0;
    const rowItems3: number[] = [...Array(Rows)].map(() => {
        return (incrementor += 3);
    });
    incrementor = 0;
    const rowItems4: number[] = [...Array(Rows)].map(() => {
        return (incrementor += 4);
    });
    incrementor = 0;
    const rowItems5: number[] = [...Array(Rows)].map(() => {
        return (incrementor += 5);
    });
    incrementor = 0;
    const rowItems6: number[] = [...Array(Rows)].map(() => {
        return (incrementor += 6);
    });
    incrementor = 0;
    const rowItems7: number[] = [...Array(Rows)].map(() => {
        return (incrementor += 7);
    });
    incrementor = 0;
    const rowItems8: number[] = [...Array(Rows)].map(() => {
        return (incrementor += 8);
    });
    incrementor = 0;
    const rowItems9: number[] = [...Array(Rows)].map(() => {
        return (incrementor += 9);
    });
    incrementor = 0;
    const rowItems10: number[] = [...Array(Rows)].map(() => {
        return (incrementor += 10);
    });

    console.log(rowItems);

    function subtractFirstCols() {
        rowItems.length--;
    }

    function subtractFirstRows() {
        cols.length--;
    }
    function subtractTheRestOfCols() {
        rowItems2.length--;
        rowItems3.length--;
        rowItems4.length--;
        rowItems5.length--;
        rowItems6.length--;
        rowItems7.length--;
        rowItems8.length--;
        rowItems9.length--;
        rowItems10.length--;
    }
    function subtractTheRestOfRows() {
        cols2.length--;
        cols3.length--;
        cols4.length--;
        cols5.length--;
        cols6.length--;
        cols7.length--;
        cols8.length--;
        cols9.length--;
        cols10.length--;
    }
</script>
<h1 class="caption">Times Table</h1>

<div class="outer-box">
    <div
        class="row-item"
        contenteditable="true"
        bind:textContent={rowItems[0]}
    />
    {#each rowItems as rowItem}
        <div
            class="row-item"
            contenteditable="true"
            bind:textContent={rowItem}
        />
    {/each}
</div>
<div class="top-box1">
    {#each cols as col}
        <div class="row" contenteditable="true" bind:textContent={col}>
            {#each rowItems as rowItem}
                <div
                    class="row-item"
                    contenteditable="true"
                    bind:textContent={rowItem}
                />
            {/each}
        </div>
    {/each}
</div>

<div class="top-box2">
    {#each cols as col}
        <div class="row" contenteditable="true" bind:textContent={col}>
            {#each rowItems as rowItem}
                <div
                    class="row-item"
                    contenteditable="true"
                    bind:textContent={rowItem}
                />
            {/each}
        </div>
    {/each}
</div>

<div class="outer-box2">
    {#each cols2 as col2}
        <div class="row" contenteditable="true" bind:textContent={col2}>
            {#each rowItems2 as rowItem2}
                <div
                    class="row-item2"
                    contenteditable="true"
                    bind:textContent={rowItem2}
                />
            {/each}
        </div>
    {/each}
</div>
<div class="outer-box3">
    {#each cols3 as col3}
        <div class="row" contenteditable="true" bind:textContent={col3}>
            {#each rowItems3 as rowItem3}
                <div
                    class="row-item"
                    contenteditable="true"
                    bind:textContent={rowItem3}
                />
            {/each}
        </div>
    {/each}
</div>

<div class="outer-box4">
    {#each cols4 as col4}
        <div class="row" contenteditable="true" bind:textContent={col4}>
            {#each rowItems4 as rowItem4}
                <div
                    class="row-item2"
                    contenteditable="true"
                    bind:textContent={rowItem4}
                />
            {/each}
        </div>
    {/each}
</div>
<div class="outer-box5">
    {#each cols5 as col5}
        <div class="row" contenteditable="true" bind:textContent={col5}>
            {#each rowItems5 as rowItem5}
                <div
                    class="row-item"
                    contenteditable="true"
                    bind:textContent={rowItem5}
                />
            {/each}
        </div>
    {/each}
</div>

<div class="outer-box6">
    {#each cols6 as col6}
        <div class="row" contenteditable="true" bind:textContent={col6}>
            {#each rowItems6 as rowItem6}
                <div
                    class="row-item2"
                    contenteditable="true"
                    bind:textContent={rowItem6}
                />
            {/each}
        </div>
    {/each}
</div>
<div class="outer-box7">
    {#each cols7 as col7}
        <div class="row" contenteditable="true" bind:textContent={col7}>
            {#each rowItems7 as rowItem7}
                <div
                    class="row-item"
                    contenteditable="true"
                    bind:textContent={rowItem7}
                />
            {/each}
        </div>
    {/each}
</div>

<div class="outer-box8">
    {#each cols8 as col8}
        <div class="row" contenteditable="true" bind:textContent={col8}>
            {#each rowItems8 as rowItem8}
                <div
                    class="row-item2"
                    contenteditable="true"
                    bind:textContent={rowItem8}
                />
            {/each}
        </div>
    {/each}
</div>
<div class="outer-box9">
    {#each cols9 as col9}
        <div class="row" contenteditable="true" bind:textContent={col9}>
            {#each rowItems9 as rowItem9}
                <div
                    class="row-item"
                    contenteditable="true"
                    bind:textContent={rowItem9}
                />
            {/each}
        </div>
    {/each}
</div>
<div class="outer-box10">
    {#each cols10 as col10}
        <div class="row" contenteditable="true" bind:textContent={col10}>
            {#each rowItems10 as rowItem10}
                <div
                    class="row-item2"
                    contenteditable="true"
                    bind:textContent={rowItem10}
                />
            {/each}
        </div>
    {/each}
</div>
<div class="changers">
<li class="changer" on:click={subtractFirstCols}>subtractFirstCols</li>
<li class="changer" on:click={subtractFirstRows}>subtractFirstRows</li>
<li class="changer" on:click={subtractTheRestOfCols}>
    subtractTheRestOfCols
</li>
<li class="changer" on:click={subtractTheRestOfRows}>
    subtractTheRestOfRows
</li>
</div>
<style>
   :global(body){
    background-color: black;
   }

    .caption {
        text-align: center;
        color: #c23434;
    }
    .top-box1,
    .top-box2,
    .outer-box2,
    .outer-box3,
    .outer-box4,
    .outer-box5,
    .outer-box6,
    .outer-box7,
    .outer-box8,
    .outer-box9,
    .outer-box10 {
        width: 90%;
        float: right;
        background-color: rgb(50, 50, 201);
    }
    .top-box1 > div:first-child {
        font-weight: bolder;
        color: #c23434;
        font-size: larger;
    }
    .outer-box {     
        display: flex;
        flex-direction: column;
         width: 10%;
         background-color: green;
        font-weight: bolder;
        color: #c23434;
        font-size: medium;

        float: left;
    }
    .row {
        display: flex;
    }
    .row-item {
        border: solid black;
        flex: 1;
        text-align: center;
    }
    .row-item2 {
        border: solid black;
        flex: 1;
        text-align: center;
    }
    .changers{
       position: fixed;
       bottom: 310px;
       color:rgb(45, 145, 112);
    }

    .changer{ 
        position:relative;
        cursor: pointer;
    }
</style>
