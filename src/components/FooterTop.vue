<template>
    <div class="backgroundContainer">
        <div class="bigContainer">
            <div class="linkContainer">
            <div>
                <DcComicsComponent/>
            </div>
            <div>
                <ShopComponent/>
            </div>
            <div>
                <DcComponent/>
            </div> 
            <div>
                <SitesComponent/>
            </div>           
            </div>
            <div class="footerLogoContainer">

            </div>
        </div>
        
        
    </div>
</template>

<script>
import DcComicsComponent from './FootersComponent/DcComicsComponent.vue'
import ShopComponent from './FootersComponent/ShopComponent.vue'
import DcComponent from './FootersComponent/DcComponent.vue'
import SitesComponent from './FootersComponent/SitesComponent.vue'

export default {
    name: 'FooterTop',
    components: {
        DcComicsComponent,
        ShopComponent,
        DcComponent,
        SitesComponent
    }
}
</script>

<style scoped lang="scss">
.backgroundContainer{
    height: 400px;
    background-image: url('../assets/img/footer-bg.jpg');
}

.bigContainer{
    width: 80%;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
}

.linkContainer{
    height: 400px;
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
}
</style>