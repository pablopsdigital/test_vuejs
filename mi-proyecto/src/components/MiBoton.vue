<template>
<div class="MiBoton">
    <h1>Ejemplo condicional</h1>
    {{visible}}
    <div v-if='visibleBooleano'>
      Usuario autenticado <button :style="btnStyles">{{textoBoton}}</button>
    </div>
    <div v-if="cadenaTexto == 'clave'">
        Usuario autenticado <button :style="btnStyles">{{textoBoton}}</button>
    </div>

</div>
</template>

<script>
export default {
    name:'MiBoton',
    data() {
        return {
            visibleBooleano:true,
            cadenaTexto:'clave'
        }
    },
    props:{
        textoBoton:String,
        color:String
    },
    computed: {
        btnStyles() {
            return {
                "background-color": this.color,
            };
        }
    },
    
}
</script>

<style>

</style>