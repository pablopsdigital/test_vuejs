<template>
    <div class="card col-md-4">
        <div class="card-body">
        <h5 class="card-title">Opción 3  {{estado}}</h5>

        <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse rhoncus tristique nibh id tincidunt.  Aenean nisi massa, scelerisque vel lacus a, fermentum lacinia tellus.</p>
        <button class="btn btn-primary">Opción 1</button>
        <input @keypress="estado='teclado'" @keypress.a="estado='tecla a'">
        <a  v-on:click="estado='click'" v-on:mouseover="estado='hover'" class="btn btn-success">Opción 3 </a>
        </div>
    </div>
</template>

<script>
export default {
    name:'Box3',
    data() {
        return {
            estado:''
            
        }
    },
}
</script>