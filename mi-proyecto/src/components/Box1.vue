<template>
    <div class="card col-md-4 pl-1">
        <div class="card-body">
        <h5 class="card-title">Opción 1: {{opcion}}</h5>

        <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse rhoncus tristique nibh id tincidunt.  Aenean nisi massa, scelerisque vel lacus a, fermentum lacinia tellus.</p>
        <button class="btn btn-primary" v-on:click='sumar'>Opción 1</button>
        </div>
    </div>
</template>

<script>
export default {
    name:'Box1',
    data(){
        return{
            opcion:''
        }
    },
    methods: {
        sumar: function(){
            this.opcion = Math.floor(Math.random()*1000);

        }
        
    },
    
}
</script>