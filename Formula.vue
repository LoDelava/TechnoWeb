<template>
   <form action="" method="post">
    <div>
        <label for="name">Nom :</label>
        <input type="text" id="name" name="user_name">
    </div>
    <div>
        <label for="surname">Prenom :</label>
        <input type="text" id="surname" name="user_surname">
    </div>
    <div>
        <label for="mail">e-mail :</label>
        <input type="email" id="mail" name="user_mail">
    </div>
    <div>
        <label for="date">Date de naissance</label>
        <input type="date" id="date" name="date_nai">
    </div>
    <div>
        <label for="phone">numero de telephone</label>
        <input type="number" id="phone">
    </div>
    <div>
        <label for="gender">Sexe :</label>
        <input type="radio" id="sex" name="user_sex"/>
    </div>
    </form> 
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