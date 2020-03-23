<template>
        <div class="nav-bar">
            <router-link class="nav-button" :to="{ name: 'Accueil'}"><h3>Accueil</h3></router-link>
            <router-link class="nav-button" :to="{ name: 'Formulaire'}"><h3>Formulaire</h3></router-link>
            <router-link class="nav-button" :to="{ name: 'About'}"><h3>About</h3></router-link>
            <h1> Bienvenue </h1>
        </div>
        

        
</template>
<script>
export default {
    name: 'App',
    data: function() {
        return {
        
        }
    },

}
</script>

<style>

</style>