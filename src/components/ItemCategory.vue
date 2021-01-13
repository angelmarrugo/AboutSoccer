<template>
    <div class="item-category text-center text-white position-relative">
        <div class="item-category__rectangle mx-auto">
            <img src="../assets/bg_category03.svg" class="img-fluid " alt="icon-category" >
        </div>
        <h5 class="item-category-title mt-4">{{name}}</h5>
        <p class="item-category-description">{{description}}</p>
    </div>
</template>

<script>
    export default {
        props: ['id', 'name', 'description', 'image'],
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
    .item-category{
    width: 50% !important;
}

.item-category__rectangle{
    width:7rem !important;
    height: 7.3rem !important;
    padding: .9rem !important;
}
  }

@media (min-width: 576px) and (max-width: 767.98px) {
    .item-category{
    width: 50% !important;
}
  }

@media (min-width: 768px) and (max-width: 991.98px) { 
   .item-category__rectangle{
    width:5rem !important;
    height: 5.3rem !important;
    padding: .9rem !important;
}
 }

@media (min-width: 992px) and (max-width: 1199.98px) {  }

@media (min-width: 1200px) { 
    
 }

.item-category{
    width: 25%;
    padding: 1rem;
}

.item-category__rectangle {
    width:8rem;
    height: 8.3rem;
    border-radius: 0.9rem;
    background-color:#2D2D2D; 
    padding: 2rem;
    cursor: pointer;
    animation: in .3s;
    
}


@keyframes in {
    from   { -webkit-transform: rotate(45deg) scale(0.9); }
    to { -webkit-transform:  rotate(0deg) scale(1);}
}

@keyframes out {
    0%   { -webkit-transform: rotate(0deg) scale(1); }
    100% { -webkit-transform: rotate(45deg) scale(0.9); }
}

.item-category__rectangle:hover{
      animation: out .3s;
  animation-direction: normal;
   animation-fill-mode: forwards;
animation-timing-function: ease-out;  
 animation-direction: alternate;
}



.item-category-title{
    font-family: Montserrat semibold, sans-serif;
    font-size: 1rem;
}

.item-category-description{
    font-family: Montserrat-medium, sans-serif;
    font-size: .8rem;
    line-height: 1.1;
}

</style>