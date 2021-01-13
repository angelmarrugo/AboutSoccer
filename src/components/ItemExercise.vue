<template>
    <div class="card-content" style=" ">
        <img v-bind:src="img" class="img-fluid" alt="Responsive image">
        <p class="text-description p-3">{{description}}</p>
    </div>
</template>

<script>
import img from '@/assets/img_exercise.png';
export default {
    
    props: ['description','img_exercise'],
    data() {
        return {
            img 
        }
    },
}
</script>

<style scoped>
    .text-description {
        font-family: Montserrat-bold, sans-serif !important;
        color: #1B1A1A;
        font-size: 0.87rem;
        background-color: white;
    }

    .card-content{
    border-radius:1.5rem;
    box-shadow: 1px 2px 4px 2px rgba(0, 0, 0, 0.2), 1px 3px 5px 1px rgba(252, 254, 255, 0.19);
    }
</style>