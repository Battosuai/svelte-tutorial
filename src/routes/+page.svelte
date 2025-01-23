<script lang='ts'>
	import Nested from "../components/Nested.svelte";

	let name = "asif";
	let src = 'https://placehold.co/600x400'
</script>

<h1>Welcome to Svelte, {name}</h1>
<h2>Manipulation: {name.toUpperCase()}</h2>

<br>

<img {src} alt="{name} dances"/>

<Nested />

<p>Test</p>

