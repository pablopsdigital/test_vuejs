<template>
    <ul class="nav">
        <item-menu v-bind:navegacionData = "{texto:'Inicio', url:'/inicio'}"/>
        <item-menu v-bind:navegacionData = "{texto:'Acerca', url:'/acerca'}"/>
        <item-menu v-bind:navegacionData = "{texto:'Tienda', url:'/tienda'}"/>
        <item-menu v-bind:navegacionData = "{texto:'Contacto', url:'http://pablopsdigital.com'}"/>
    </ul>
</template>

<script>
    //import componets
    import ItemMenu from './ItemMenu.vue'

    export default {
        name:'MiMenu',
        components: {
            ItemMenu //Registro componentes

        },
        data() {
            return {

            }
        },
    }
</script>


<style>
</style>