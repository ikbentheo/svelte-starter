<script lang="ts">
	import '../app.css';
	import '../fonts.css';
	let { children } = $props();
</script>

<div class="font-roboto">
	{@render children()}
</div>

