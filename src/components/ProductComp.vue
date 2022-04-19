<template>
    <div class="product">
        <div class="box">
            <img :src="src" alt="copertina">
            <h3>{{ titolo }}</h3>
        </div>
    </div>
</template>

<script>
    export default{
        name: 'ProductComp',
        props: {
            src: String,
            titolo: String
        }
    }
</script>

<style scoped lang="scss">
    .product{
        width: 80%;
        margin: 0 auto;
        margin-top: 20px;
        //display: flex;
        //flex-basis: calc((100% / 6) - 8px);
        border: 1px solid black;

        .box{
            //background-color: white;
            img{
                max-width: 100%;
            }
        }
    }

</style>
