<template>
    <div>
        <h3>Shop</h3>
        <ul>
            <li v-for="(element, index) in menuShop" :key='index'>
                <a :href="`${element.url}`"> {{ element.name }}</a>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'ShopComponent',
    data() {
        return {
            menuShop: [
                {
                    name: 'Shop DC',
                    url: '/shopdc'
                },
                {
                    name: 'Shop DC Collectibles',
                    url: '/shopdccollectibles'
                },
            ]
        }
    }
}
</script>

<style scoped lang="scss">

h3{
    color: white;
}

ul{
    padding-inline-start: 0;
    margin-block-start: 0;
}

li{
    list-style-type: none;
    margin: 0 15px;
}

a{
    text-decoration: none;
    color: white;
}
</style>