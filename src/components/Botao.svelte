<script lang="ts"> //Pode se usar TypeScript.
    export let texto: string
    export let triplo: boolean = false
    export let duplo: boolean = false
    export let operacao: boolean = false
    export let destaque: boolean = false
    export let onClick: (valor: string) => void = () => {}

    function click() {
        console.log('click...')
    }
</script>

<button class="botao" 
    on:click={() => onClick(texto)}
    class:triplo class:duplo class:operacao class:destaque>
    {texto}
</button>

<style>
    .botao {
        flex-basis: 25%;
        margin: 0;
        border: 1px solid var(--cor-fundo);
    }

    .triplo {
        flex-basis: 75%;
    }

    .duplo {
        flex-basis: 50%;
    }

    .operacao {
        background-color: rgb(0, 140, 255);
        color: white;
    }

    .destaque {
        background-color: rgb(255, 0, 0);
        color: white;
    }
</style>