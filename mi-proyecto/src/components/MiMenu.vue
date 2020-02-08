<template>
    <ul class="nav">
        <li class="nav-item">
            <a class="nav-link" v-bind:class="{active: claseActivo}" href="#">Active</a>
        </li>
         <li class="nav-item">
            <a class="nav-link" href="#">Link</a>
        </li>
        <li class="nav-item">
            <a class="nav-link" href="#">Link</a>
        </li>
        <li class="nav-item">
            <a class="nav-link disabled" href="#">Disebled</a>
        </li>
    </ul>
</template>


<script>
    export default {
        name:'MiMenu',
        data() {
            return {
                claseActivo:true    
            }
        },
    }
</script>


<style>
    .active{
        font-weight: bold
    }

</style>