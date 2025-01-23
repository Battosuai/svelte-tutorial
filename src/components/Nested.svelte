<script>
	let count = $state(0);

	let numbers = $state([1, 2, 3, 4, 5]);

	let total = $derived(numbers.reduce((a, b) => a + b, 0));

	function increment() {
		count++;
	}

	function addNumber() {
		numbers.push(numbers.length);
	}
</script>

<p>This is a nested component</p>

<button onclick={increment}>
	Clicked {count}
	{count === 1 ? 'time' : 'times'}
</button>

<button onclick={addNumber}>
	{numbers.join(' + ')} = {total}
</button>

<style>
    p {
        color: goldenrod;
        font-family: 'Comic Sans MS', cursive;
        font-size: 2em;
    }

    button {
        color: goldenrod;
        font-size: 1.2rem;
        padding: 0.5rem 1rem;
        border: 1px solid goldenrod;
    }
</style>