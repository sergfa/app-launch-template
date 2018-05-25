<template>
    <section id="about" class="bg-primary py-5">
        <div class="container">
            <div class="row align-items-center mb-5">
                <div class="col text-center">
                    <h1 class="text-uppercase font-weight-bold">About</h1>
                </div>
            </div>
            <div class="row">
                <div class="col-lg-6 d-flex mb-3" v-for="(item, index) in items" :key="index">
                    <img :src="item.image"  alt="about" class="img-fluid img-thumbnail rounded about-image mr-5">
                    <p class="align-self-center lead">{{item.text}}</p>    
                </div>
            </div>
        </div>
    </section>
</template>
<script>
import itemImage1 from '../assets/food.jpg'

export default {
    data () {
        return {
            items: [{image: itemImage1, text: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quas ipsam eos nesciunt inventore quia consequuntur enim ex deserunt veniam odit.'},
            {image: itemImage1, text: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quas ipsam eos nesciunt inventore quia consequuntur enim ex deserunt veniam odit.'},
            {image: itemImage1, text: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quas ipsam eos nesciunt inventore quia consequuntur enim ex deserunt veniam odit.'},
            {image: itemImage1, text: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quas ipsam eos nesciunt inventore quia consequuntur enim ex deserunt veniam odit.'}]
        }
    }    
}
</script>

<style scoped>
.about-image {
    width: 175px;
    height: 175px;;
}
</style>
