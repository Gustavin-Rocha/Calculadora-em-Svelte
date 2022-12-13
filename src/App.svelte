<script lang="ts">
    import Calculadora from "./components/Calculadora.svelte";
</script>

<main>
	<Calculadora />
</main>

<style>
	:global(body) {
		background-image: url('../vetores/math.jpg');
	}
	
	:root {
		--cor-fundo: rgb(0, 0, 0);
	}

	main {
		display: flex;
		justify-content: center;
		align-items: center;
		height: 90vh;
	}
</style>