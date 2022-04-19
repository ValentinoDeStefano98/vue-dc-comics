<template>
    <div>
       <ul>
           <li v-for="(element, index) in menuNav" :key="index" v-on:click="active">
               <a :href="`${element.url}`"> {{ element.title }} </a>
           </li>

       </ul>
    </div>
</template>

<script>
export default {
    name: 'HeaderNavComponent',
    data(){
        return{
            menuNav: [
                {
                    title: 'Characters',
                    url: '#'
                },
                {
                    title: 'Comics',
                    url: '#'
                },
                {
                    title: 'Movies',
                    url: '#'
                },
                {
                    title: 'TV',
                    url: '#'
                },
                {
                    title: 'Games',
                    url: '#'
                },
                {
                    title: 'Collectibles',
                    url: '#'
                },
                {
                    title: 'Videos',
                    url: '#'
                },
                {
                    title: 'Fans',
                    url: '#'
                },
                {
                    title: 'News',
                    url: '#'
                },
                {
                    title: 'Group',
                    url: '#'
                },
            ]
        }
    }
}
</script>

<style scoped lang="scss">
ul{
    display: flex;
}

li{
    list-style-type: none;
    margin: 0 15px;
    text-transform: uppercase;
    font-weight: bold;
}

a{
    text-decoration: none;
    color: black;
}

.active{
    color: #0282F9;
    border-block-end: 1px solid black;
}
</style>