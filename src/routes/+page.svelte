<script>
    let stack = ['svelte', 'taildwind css', 'shadcn', 'gsap']
</script>

<main class="flex flex-col items-center justify-center w-screen h-screen ">
    <h1 class="text-2xl font-bold">Theo Starter Template</h1>
    Stack
    <ul>
        {#each stack as item}
            <li class="px-2 py-1 my-2 font-bold text-center text-white bg-blue-400 up rounded-xl">{item}</li>
        {/each}
    </ul>
</main>