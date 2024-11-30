<script>
	import Button from "$lib/components/ui/button/button.svelte";
	import Buttons from "./components/Buttons.svelte";
	import Colors from "./components/Colors.svelte";
	import Text from "./components/Text.svelte";
</script>

<main class="w-full grid grid-cols-1 md:grid-cols-3 lg:grid-cols-4 p-4 gap-4">
    <Text />
    <Buttons />
    <Colors />
</main>
