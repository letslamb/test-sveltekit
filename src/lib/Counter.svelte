<script>
  import { writable } from 'svelte/store'

	let count = writable(0);

	function increment() {
		count.update(n => n + 1);
	};
</script>

<button on:click={increment}>
	Clicks: {$count}
</button>

<style>
	button {
		font-family: inherit;
		font-size: inherit;
		padding: 1em 2em;
		color: #ff3e00;
		background-color: rgba(255, 62, 0, 0.1);
		border-radius: 2em;
		border: 2px solid #ff3e00;
		outline: none;
		width: 200px;
		height: 60px;
		font-variant-numeric: tabular-nums;
	}

	button:hover {
		border: 3px solid #ff3e00;
	}

	button:active {
		background-color: rgba(255, 62, 0, 0.2);
	}
</style>
