<template>
    <div class="container">
        <div class="jumbo">
            <div class="buttonContainer">
                <span class="currentSeries">Current Series</span>
            </div>
            
        </div>
        <div class="top">
            <h2> -- Content goes here -- </h2>
        </div>
    </div>
    
</template>

<script>
export default {
    name: 'MainTop',
}
</script>

<style scoped lang="scss">
.top{
    color: white;
    background-color: black;
    height: 100px;
    padding: 20px 0;
}

.jumbo{
    background-image: url(../assets/img/jumbotron.jpg);
    height: 300px;
    text-align: start;
}

.currentSeries{
    display: inline-block;
    margin-top: 280px;
    color: white;
    background-color: #0282F9;
    padding: 10px;
    text-transform: uppercase;
    font-weight: bold;
}

.buttonContainer{
    width: 80%;
    margin: 0 auto;
}
</style>