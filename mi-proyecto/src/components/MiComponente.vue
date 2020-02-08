<template>
<div class="MiComponente">
    <h1>{{libro.titulo}}</h1>
    <h2>{{libro.autor}}</h2>
    <div>
        <h3>Capítulos</h3>
        <ul>
            <li v-for="capitulo in libro.capitulos" :key="capitulo">{{capitulo}}</li>
        </ul>
    </div>

    <div>
        <h3>Estructura</h3>
        <div v-for="pagina in libro.estructura" :key="pagina">
            <p>Número de página: {{pagina.numpag}}</p>
            <p>Contenido: {{pagina.contenido}}</p>
            <p>----------------------------------------------------------</p>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name: 'MiComponente',
    data() {
        return {
            colores: ['rojo', 'verde', 'amarillo'],
            libro: {
                titulo: 'El método Lean Startup',
                autor: 'Eric Ries',
                capitulos: ['capitulo 1','capitulo 2', 'capitulo 3', 'capitulo 4'],
                estructura: [
                    {numpag:'15', contenido:"Curabitur mollis vitae ligula ut porttitor. Vestibulum lacus urna"},
                    {numpag:'25', contenido:"Curabitur mollis vitae ligula ut porttitor. Vestibulum lacus urna"},
                ]
            }
        };
    },
}
</script>

<style>

</style>
