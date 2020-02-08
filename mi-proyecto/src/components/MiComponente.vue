<template>
    <div class="MiComponente">
        <h1>{{libro.titulo}}</h1>
        <h2>{{libro.autor}}</h2>
    </div>
</template>

<script>
    export default {
        name:'MiComponente',
        data() {
            return {
                libro:{
                    titulo:'El método Lean Startup',
                    autor:'Eric Ries'
                }
            }
        },
    }
</script>


<style>

</style>