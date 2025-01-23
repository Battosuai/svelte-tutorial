<script lang="ts">
	import "../app.css";

	let { children } = $props();
</script>

<div class="min-h-screen min-w-screen-lg">
	{@render children()}
</div>
