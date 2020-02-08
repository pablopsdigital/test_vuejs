<template>

    <div>
        <div class="jumbotron">
            <h1 class="display-4">Vuejs</h1>
        </div>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse rhoncus tristique nibh id tincidunt. Aenean nisi massa, scelerisque vel lacus a, fermentum lacinia tellus. Sed lobortis dui libero, ut pulvinar ipsum vestibulum quis. Maecenas sit amet massa ut leo varius vehicula at quis purus. Fusce eu diam sit amet sapien consectetur luctus. Vestibulum tortor ligula, suscipit et tempus et, suscipit vitae arcu. Integer sed dapibus mi. Aliquam iaculis mauris sed velit placerat tincidunt. Sed aliquet dapibus rutrum. Sed lectus nibh, suscipit sit amet viverra sagittis, euismod ac velit.</p>

        <div class="row">
            <box1/>
            <box2/>
            <box3/>
        </div>
    </div>
    
</template>

<script>
import Box1 from './Box1'
import Box2 from './Box2'
import Box3 from './Box3'

export default {
    name:'contenido',
    data() {
        return {
            
        }
    },
    components:{
        Box1,
        Box2,
        Box3
    }
}
</script>

<style scoped>

</style>