<template>
    <div>
        <li class="nav-item" v-bind:style="{backgroundColor:colorRandom}">
            <!--Link menu si está o no activo, cargar atributos html en este caso ref y carga de texto normal-->
            <a class="nav-link" v-bind:class="{active: claseActivo}" v-bind:href="navegacionData.url">{{navegacionData.texto}}</a>
        </li>
    </div>
</template>

<script>
export default {
    name:'ItemMenu',
    data() {
        return {
            claseActivo:true,
            colorRandom: '#' + Math.floor(Math.random()*6777215).toString(16)
        }
    },
    props:{
        navegacionData:Object, //Definir propiedades del componente
    },
}
</script>

<style>
    .active{
        font-weight: bold
    }
</style>