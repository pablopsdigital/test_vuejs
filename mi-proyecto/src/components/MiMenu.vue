<template>
    <ul class="nav">
        <!--Cargar items en base a un array de datos-->
        <item-menu v-bind:navegacionData="item" :key='item' v-for="item in itemsDeNavegacion"/>
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
                //Array with objects for menu
                itemsDeNavegacion: [
                    {texto:'Inicio', url:'/inicio'},
                    {texto:'Acerca', url:'/acerca'},
                    {texto:'Tienda', url:'/tienda'},
                    {texto:'Contacto', url:'http://pablopsdigital.com'}
                ]
            }
        },
    }
</script>


<style>
</style>