<template>

    <div class="card-modulo rounded " style="background-color:#EEEEEE; position:relative">
        <h5 class="card-modulo-title  text-left">{{name}}</h5>
        <img  v-if="active" src="../assets/../assets/bg_mark_ball_kill.svg"  style="position:absolute; left:0;bottom:0;width:8.1rem;">
        <img v-if="!active" src="../assets/../assets/bg_mark_ball.svg" style="position:absolute; left:0;bottom:0;width:8.1rem;">
        <h5 class="card-modulo-footer text-right">{{count}}</h5>
    
    </div>

</template>

<script>
    export default {

        props: ['name', 'count', 'active'],
        data() {
            return {
            }
        },
        mounted() {
        //addClassNameListener("card-modulo", function(){alert("Hello");});
        },

        computed: {
           
        },
        methods: {
             
        },
    }
</script>

<style scoped>

@media (max-width: 575.98px) { 
    .card-modulo{
        min-width: 75% !important;
        height: 10rem !important;
    }
 }

@media (min-width: 576px) and (max-width: 767.98px) { 
    .card-modulo{
        min-width: 65% !important;
    }
 }

@media (min-width: 768px) and (max-width: 991.98px) {  
    .card-modulo{
        min-width: 50% !important;
    }
}

@media (min-width: 992px) and (max-width: 1199.98px) {
    .card-modulo{
        min-width: 40% !important;
    }
  }

@media (min-width: 1200px) {  }

    .card-modulo {
        float: left;
        width: 75.333%;
        height: 12rem;
        padding: 1.85rem;
        margin-right: 1.3rem;
        margin-bottom: 2rem;
        border: 0;
        cursor: pointer;
    }

    .card-modulo.active {
        border: 2px solid #FF0313;
        color: #FF0313;
    }

    .card-modulo.active>* {
        color: #FF0313;
    }

    .card-modulo-title {
        font-family: Montserrat semibold, sans-serif;
        color: #8D8D8D;
        font-size: 1.4rem;
    }

    .card-modulo-title.active {
        font-family: Montserrat semibold, sans-serif;
        color: #FF0313;
        font-size: 1.4rem;
    }

    .card-modulo-footer {
        font-family: Montserrat semibold, sans-serif;
        color: #8D8D8D;
        font-size: 1.2rem;
        position: absolute;
        bottom: 0;
        right: 0;
        margin: 1.85rem;
    
    }

    .content-card-modulo {
        align-items: stretch;
        display: flex;
        flex-direction: row;
        flex-wrap: nowrap;
        overflow-x: scroll;
        overflow-y: hidden;
          scrollbar-width: none;
    }
</style>