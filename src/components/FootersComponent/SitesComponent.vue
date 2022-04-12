<template>
    <div>
        <h3>DC</h3>
        <ul>
            <li v-for="(element, index) in menuSites" :key='index'>
                <a :href="`${element.url}`"> {{ element.name }}</a>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'SitesComponent',
    data() {
        return {
            menuSites: [
                {
                    name: 'DC',
                    url: '/dc'
                },
                {
                    name: 'MAD Magazine',
                    url: '/mad-magazine'
                },
                {
                    name: 'DC Kids',
                    url: '/dc-kids'
                },
                {
                    name: 'DC Universe',
                    url: '/dc-universe'
                },
                {
                    name: 'DC Power Visa',
                    url: '/dc-power-visa'
                }
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