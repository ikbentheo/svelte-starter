<script>
	import { Button as ButtonPrimitive } from "bits-ui";
	import Icon from '@iconify/svelte';
	import { buttonVariants } from "./index.js";
	import { cn } from "$lib/utils.js";
	let className = undefined;
	export let variant = "default";
	export let size = "default";
	export let builders = [];
	export { className as class };
	export let icon
</script>

<ButtonPrimitive.Root
	{builders}
	class={cn(buttonVariants({ variant, size, className }))}
	type="button"
	{...$$restProps}
	on:click
	on:keydown
>
{#if icon}
<Icon class="w-full h-full m-1.5" icon={icon} />
{/if}
	<slot />
</ButtonPrimitive.Root>
