<script>
    export default {
        data() {
        return {
            title: " --> Content goes here<--",
            slideImmagini: []
        }
    }  
    }
</script>


<template lang="">
    <div class="corpo">
        <div class="corpoPagina">
            <h2>{{title}} </h2>
        </div>
    </div>
</template>


<style lang="scss">
    @use './src/styles/partials/_variables.scss' as *;
    @use './src/styles/partials/_mixins.scss' as *;

    .corpo{
        background-color: black;
        height: 150px;
        padding: 40px 0;


        .corpoPagina{
            @include width70;
            color: white;
        }

    }
</style>