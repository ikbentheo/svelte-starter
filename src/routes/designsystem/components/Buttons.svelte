<script>
	import Button from "$lib/components/ui/button/button.svelte";

    
</script>

<div class="border rounded-3xl border-dashed col-span-1 flex flex-col flex-grow gap-2 p-4 items-start">
    <p class="mb-2 text-xs font-bold">Buttons</p>
    <Button>Default</Button>
    <Button variant="secondary">Secondary</Button>
    <Button variant="ghost">Ghost</Button>
    <Button variant="outline">Outline</Button>
</div>