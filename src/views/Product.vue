<template>
    <v-container>
        <h1>Product</h1>
        <v-row>
            <v-btn fab class="ma-2" color="primary" v-on:click="addProducts">
                <v-icon>mdi-plus</v-icon>
            </v-btn>
            <p class="pt-6">Ajouter un produit</p>
        </v-row>
        <AddProduct v-if="add"></AddProduct>
    </v-container>
</template>

<script>
    import AddProduct from "../components/AddProduct";
    export default {
        name: "Product",
        components: {
            AddProduct
        },
        data () {
            return {
                add: false
            }
        },
        methods: {
            addProducts () {
                this.add = this.add === false
            }
        }
    }
</script>

<style scoped>

</style>
