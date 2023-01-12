<script>
export default {
    data() {
        return {
            activeItem: 0,
            logo: "src/assets/img/dc-logo.png",
            nav: [
                {
                    label: 'CHARACTERS',
                    url: '#',
                    active: false
                },
                {
                    label: 'COMICS',
                    url: '#',
                    active: true
                },
                {
                    label: 'MOVIES',
                    url: '#',
                    active: false
                },
                {
                    label: 'TV',
                    url: '#',
                    active: false
                },
                {
                    label: 'GAMES',
                    url: '#',
                    active: false
                },
                {
                    label: 'COLLECTIBLES',
                    url: '#',
                    active: false
                },
                {
                    label: 'VIDEOS',
                    url: '#',
                    active: false
                },
                {
                    label: 'FANS',
                    url: '#',
                    active: false
                },
                {
                    label: 'NEWS',
                    url: '#',
                    active: false
                },
                {
                    label: 'SHOP',
                    url: '#',
                    active: false
                }
            ]
        }
    },
    methods:{
        changeItem(index){
            this.activeItem = index
        },
    }
}
</script>

<template lang="">
    <header>
       <a href="/" class="logo">
            <img :src="logo" alt="logoDc">
       </a>
        <nav>
            <ul>
                <li v-for="(item, index) in nav" :key="index" @click="changeItem(index)" > 
                    <a :href="item.url"  :class="(activeItem === index) ? 'active' : '' ">
                {{item.label}}
                    </a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss">
    @use './src/styles/partials/_variables.scss' as *;
    @use './src/styles/partials/_mixins.scss' as *;

    header{
        @include width70;
        display: flex;
        justify-content: space-between;
        padding: 30px 0 0;

        .logo{
            padding-bottom: 10px;
        }

        nav{
            display: flex;
            align-items: center;

            ul{
                @include center;
                list-style-type: none;

    
                li a {
                    display:flex;
                    align-items: center;
                    margin: 0 15px;
                    height: 120px;
                    text-decoration: none;
                    font-weight: 600;
                    font-size: 13px;
                    color: rgba(0, 0, 0, 0.75);
                    border-bottom: 5px solid white ;
                    
                
    
                    &.active,
                    &:hover {
                        color: $blue;
                        border-bottom:5px solid $blue;
                    }
                }
            }
        }

    }

</style>