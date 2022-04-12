<template>
    <div>
       <ul>
           <li v-for="(element, index) in menuNav" :key="index">
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
}

a{
    text-decoration: none;
    color: black;
}
</style>