<template>
    <div class="card-item-modulo mt-3"
     data-toggle="collapse"
                    :data-target="'#collapseModulo'+type+id" aria-expanded="true" :aria-controls="'collapseModulo'+type+id">
        <div class="card-item-modulo-header d-flex justify-content-between" :id="'headingModulo'+type+id"
        
       >
            <h2 class="mb-0 p-0  text-left text-modulo">
                {{title}}
            </h2>
            <img src="../assets/bg_arrow_down.svg" alt="icon-arrow" width="12rem">
        </div>

        <div :id="'collapseModulo'+type+id" class="collapse " :aria-labelledby="'headingModulo'+type+id" data-parent="#accordionExample">
            <div class="card-body">
                Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry richardson ad squid.
                3 wolf moon officia aute, non cupidatat skateboard dolor brunch. Food truck quinoa nesciunt
                laborum eiusmod. Brunch 3 wolf moon tempor, sunt aliqua put a bird on it squid single-origin
                coffee nulla assumenda shoreditch et. Nihil anim keffiyeh helvetica, craft beer labore wes
                anderson cred nesciunt sapiente ea proident. Ad vegan excepteur butcher vice lomo. Leggings
                occaecat craft beer farm-to-table, raw denim aesthetic synth nesciunt you probably haven't heard
                of them accusamus labore sustainable VHS.
            </div>
        </div>
    </div>

</template>

<script>
    export default {

        props: ['id','title', 'description','type'],
        data() {
            return {}
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

.card-item-modulo{
    border-radius: .3rem;
    border: #f8f8f82d;
    box-shadow: 1px 1px 2px #F8F8F8, 1px 1px 2px #D5D5D5, 1px 1px 8px#00000021;
    padding: 1.1rem 1.3rem;
    cursor: pointer;
    background-color:  white;
    
}

.text-modulo{
    font-family: Montserrat-bold, sans-serif;
    font-size: .95rem;
    color: #080808;
    padding-left: 1.3rem;
}

</style>