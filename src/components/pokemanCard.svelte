<script>
	export let pokeman;
	import { fade } from 'svelte/transition';
</script>

<a
	class="p-6  text-gray-800 text-center rounded-mod shadow-sm hover:shadow-md flex flex-col items-center"
	href={`/pokemon/${pokeman.id}`}
	transition:fade
>
	<img class="h-40 w-40" src={pokeman.image} alt={pokeman.name} />
	<h2 class="text-xl">{pokeman.id}. {pokeman.name}</h2>
</a>
