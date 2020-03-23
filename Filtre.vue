<template>
    <div>
    <br>
    <input v-model="texte"  placeholder="Entrer texte"/>

    {{texte|majusculesTexte}}

    </div>
</template>
<script>
export default {
    name: 'App',
    data: function() {
        return {
            texte: "exemple",
        }
    },
 filters: {
     majusculesTexte: function(texte) {
        return texte.toUpperCase()
        }
    }
}
</script>

<style>

</style>