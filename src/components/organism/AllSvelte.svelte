<script>
	import Pokemon from '../atoms/Pokemon.svelte';
	import Thing from '../../Thing.svelte';



	let count  = 0;
	$: double = count * 2;

	const increment = () => {
		count++;
	};


	$: {
		console.log(double);
	}


	let things = [
		{ id: 1, name: 'apple' },
		{ id: 2, name: 'banana' },
		{ id: 3, name: 'carrot' },
		{ id: 4, name: 'doughnut' },
		{ id: 5, name: 'egg' },
	];

	function handleClick() {
		things = things.slice(1);
	}


	let m = { x: 0, y: 0 };

	function handleMousemove(event) {
		m.x = event.clientX;
		m.y = event.clientY;
	}


	function handleSayHello({detail}) {
		alert(detail.text);
	}

	let name = 'world';
</script>



<main>
	<h1>Hello {name}!</h1>
	<button on:click={increment}>
		{count} + 1
	</button>

	<p>
		number is { count } double is { double }
	</p>

	<button on:click={handleClick}>
		Remove first thing
	</button>
	
	{#each things as thing (thing.id)}
		<Thing name={thing.name}/>
	{/each}

	<Pokemon on:sayhello={handleSayHello}/>
	<input bind:value={name}>

	<div on:mousemove={handleMousemove}>
		The mouse on drag position is {m.x} x {m.y}
	</div>

	
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		margin: 0 auto;
		flex: 1;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 900;
	}

	p {
		color: white;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
	div { width: 100%; height: 300px; color: white; background-color: #444; }
</style>


