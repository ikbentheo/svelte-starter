<script lang="ts">
	import Button from "$lib/components/ui/button/button.svelte";


    let mousePos = $state({x: 0, y: 0})

    // Define the function outside any unrelated blocks
    function mouseMove(event: MouseEvent): void {
        mousePos.x = event.clientX
        mousePos.y = event.clientY
    }

    const menuItems = [
        { text: "Design system", link: '/designsystem' },
    ]

    const stack = [
        'Svelte 5', 'Typescript', 'Tailwindcss', 'shadCN', 'gsap', 'threlte'
    ]

    console.log("Test");
</script>

<main onmousemove={mouseMove} class="w-screen flex-col gap-4 flex items-center justify-center h-screen bg-zinc-50">


    <ul>
        {#each menuItems as menuItem}
            <li>
                <Button href={menuItem.link}>{menuItem.text}</Button>
            </li>
        {/each}
    </ul>

    <div class=" w-32 h-32 shadow-sm bg-white p-4 gap-4 font-bold rounded-2xl flex flex-col items-center justify-between">
        <h1 class="text-xs text-center">Mouse coordinates</h1>
        <div class="flex flex-col">
            <h1>y: {mousePos.y}</h1>
            <h1>x: {mousePos.x}</h1>
        </div>
    </div>

    <div class=" bg-white shadow-sm p-4 gap-4 font-bold rounded-2xl flex flex-col items-center justify-between">
        <h1 class="text-xs text-center">Stack</h1>
        <ul class="flex flex-row gap-4">
            {#each stack as item}
            <li class=" text-nowrap text-center py-2 px-2 capitalize border rounded-full">{item}</li>
            {/each}
        </ul>
    </div>



</main>