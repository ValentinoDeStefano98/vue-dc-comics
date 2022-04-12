<template>
    <div class="bottom">
        <div v-for="(element, index) in menuImg" :key="index" class="container">
            <img :src="`${element.img}`" alt="immagine">
            <h3> {{element.title}} </h3>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MainBottom',
    data(){
        return{
            menuImg: [
                {
                    img: '../assets/img/buy-comics-digital-comics.png',
                    title: 'Digital Comics'
                },
                {
                    img: '../assets/img/buy-comics-merchandise.png',
                    title: 'DC Merchandise'
                },
                {
                    img: '../assets/img/buy-comics-subscriptions.png',
                    title: 'Subscriptions'
                },
                {
                    img: '../assets/img/buy-comics-shop-locator.png',
                    title: 'Comic Shop Locator'
                },
                {
                    img: '../assets/img/buy-dc-power-visa.svg',
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