<template>
<div class="MiBoton">

    <!--If-->
    <h1>Ejemplo condicional</h1>
    <p>Valor variables: Booleano: {{visibleBooleano}}</p>
    <div v-if='visibleBooleano'>
      Usuario autenticado <button :style="btnStyles">{{textoBoton}}</button>
    </div>
    <p>-------------------------------------------------------------------------</p>
    <p>Cadena de Texto: {{cadenaTexto}}</p>
    <div v-if="cadenaTexto == 'clave'">
        Usuario autenticado <button :style="btnStyles">{{textoBoton}}</button>
    </div>

    <!--ElseIf-->
    <h1>Ejemplo condicional ElseIf</h1>
    <p>Cadena de Texto: {{cadenaTexto}}</p>
    <div v-if="cadenaTexto == 'clave'">
        Usuario autenticado <button :style="btnStyles">{{textoBoton}}</button>
    </div>
    <div v-else-if="cadenaTexto">
        <p>Dentro del else-if - El texto no es igual a {{cadenaTexto}}</p>
    </div>
    <div v-else>
        <p>Dentro else - La propiedad no existe</p>
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