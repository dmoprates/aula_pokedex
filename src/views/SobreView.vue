<template>
    <div>
        <div v-if="!pokemon.id">
            Selecione um Pokémon
        </div>
        <div v-else>
            <p>Identificador: {{ pokemon.id }}</p>
            <p>Nome: {{ pokemon.nome }}</p>
            <p>Tipo: {{ pokemon.tipo }}</p>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SobreView',
    props: {
        pokemon: Object
    }
}
</script>
