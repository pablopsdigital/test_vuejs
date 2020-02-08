<template>
    <div class="card col-md-4">
        <div class="card-body">
            <h5 class="card-title">Opción 2 - {{entradaTexto}}</h5>
            <form>
                <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse rhoncus tristique nibh id tincidunt.  Aenean nisi massa, scelerisque vel lacus a, fermentum lacinia tellus.</p>
            <div class="row">
                <input v-model="entradaTexto"/>
            </div>
            <div class="row">
                <boton class="btn btn-secondary" v-on:click="entradaTexto=''">Reset</boton>
            </div>
            </form>
        </div>
    </div>
</template>

<script>
export default {
    name:'Box2',
    data() {
        return {
            entradaTexto:''
        }
    },
    methods: {
        
    },
}
</script>