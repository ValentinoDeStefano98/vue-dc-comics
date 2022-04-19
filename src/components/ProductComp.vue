<template>
    <div class="product">
        <div class="box">
            <div class="img-container">
                <img :src="src" alt="copertina">
            </div>
            <div>
                <h3>{{ titolo }}</h3>
            </div>
            
            
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
                width: 200px;
                height: 300px;
                
            }
        }
    }

    .img-container{
        width: 200px;
        height: 200px;
        overflow: hidden;
    }

</style>
