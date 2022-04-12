<template>
    <div class="bottom">
        <div v-for="(element, index) in menuImg" :key="index" class="container">
            <img :src="`${element.img}`" alt="immagine">
            <h3> {{element.title}} </h3>
        </div>
    </div>
</template>

<script>
import image1 from '../assets/img/buy-comics-digital-comics.png';
import image2 from '../assets/img/buy-comics-merchandise.png';
import image3 from '../assets/img/buy-comics-subscriptions.png';
import image4 from '../assets/img/buy-comics-shop-locator.png';
import image5 from '../assets/img/buy-dc-power-visa.svg';

export default {
    name: 'MainBottom',
    data(){
        return{
            menuImg: [
                {
                    img: image1,
                    title: 'Digital Comics'
                },
                {
                    img: image2,
                    title: 'DC Merchandise'
                },
                {
                    img: image3,
                    title: 'Subscriptions'
                },
                {
                    img: image4,
                    title: 'Comic Shop Locator'
                },
                {
                    img: image5,
                    title: 'DC Power Visa'
                },
            ]
        }
    }
}
</script>

<style scoped lang="scss">
.bottom{
    color: white;
    background-color: #0282F9;
}

.container{
    display: flex;
    align-items: center;
}

img{
    max-width: 3%;
}
</style>