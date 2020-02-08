<template>
    <div class="card col-md-4 pl-1">
        <div class="card-body">
        <h5 class="card-title">{{texto}}</h5>

        <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse rhoncus tristique nibh id tincidunt.  Aenean nisi massa, scelerisque vel lacus a, fermentum lacinia tellus.</p>
        <button class="btn btn-primary" v-on:click="letraElegida('Opción 1')">Opción 1</button>
        <button class="btn btn-primary" v-on:click="letraElegida('Opción 2')">Opción 2</button>
        </div>
    </div>
</template>

<script>
export default {
    name:'Box1',
    data(){
        return{
            opcion:'',
            texto: 'Titular'
        }
    },
    methods: {
        sumar: function(){
            this.opcion = Math.floor(Math.random()*1000);
        },
        letraElegida: function(letra){
            this.texto = 'Pulsa el botón ' + letra
        }
    },
    
}
</script>