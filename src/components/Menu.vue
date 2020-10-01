<template>
    <v-app-bar app color="green" class="d-flex justify-center">
        <div>
            <v-btn text exact :to="{name: 'Home'}" active-class="menu-active-link" > Accueil </v-btn> |
            <v-btn text :to="{name: 'About'}" active-class="menu-active-link" > A propos </v-btn> |
            <v-btn text :to="{name: 'Product'}" active-class="menu-active-link"> Produits </v-btn>
        </div>
    </v-app-bar>
</template>

<script>
    export default {
        name: "Menu"
    }
</script>

<style lang="scss">
.v-btn {
    text-transform: none !important;
    color: white!important;
}
.menu-active-link{
    font-weight: bold!important;
}
.menu-active-link:before{
    background-color: transparent!important;
}
</style>
