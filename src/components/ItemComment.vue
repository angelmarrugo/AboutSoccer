<template>
    <div class="card-comment " style="position:relative">
       <div class="card-comment-content text-left">
            <img class="img-comment mt-2" src="../assets/img_person.png" alt="img-person">
            <p class="comment-text mt-3">{{comment}}</p>
            <h5 class="comment-autor">Andres Fernandez</h5>
            <p class="comment-type">Entraineur</p>
       </div>
    </div>
</template>

<script>
    export default {
        props: ['id', 'name', 'description', 'image'],
        data() {
            return {
                comment: 'Excellente application, cela m\'a aidé à faire tous mes entraînements'
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

<style  scoped>

@media (max-width: 575.98px) { 
      .card-comment{
        width: 95% !important;
        min-width: 95% !important;
    }
 }

@media (min-width: 576px) and (max-width: 767.98px) { 
      .card-comment{
        width: 75% !important;
        min-width: 75% !important;
    }
 }

@media (min-width: 768px) and (max-width: 991.98px) {
     .card-comment{
        width: 55% !important;
        min-width: 55% !important;
    }
  }

@media (min-width: 992px) and (max-width: 1199.98px) { 
    .card-comment{
        width: 45% !important;
        min-width: 45% !important;
    }
 }

@media (min-width: 1200px) {  }

    .img-comment{
        border-radius: 50%;
        width: 3rem;
        height: 3rem;
    }

    .card-comment-content{
        padding: .5rem 1.5rem;
        line-height: .8rem;
    }

    .card-comment{
        background-color: white;
        border-radius: 1rem;
        border: #f8f8f82d;
        box-shadow: 1px 1px 2px #F8F8F8, 1px 1px 2px #D5D5D5, 1px 1px 8px#00000021;

        float: left;
        width: 33%;
        min-width: 32%;
        margin-right: 1.3rem;
        margin-bottom: 2rem;
    }

    .comment-text{
        font-family: Montserrat-medium-italic, sans-serif;
        font-size: .7rem;
        color: #444444;
    }

    .comment-autor{
        font-family: Montserrat-bold, sans-serif;
        font-size: .9rem;
        color:#131313;
    }

    .comment-type{
        font-family: Montserrat-medium, sans-serif;
        font-size: .79rem;
        color:#BBBBBB;
    }
</style>