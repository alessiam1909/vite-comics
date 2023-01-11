<script>
export default {
    data() {
        return {
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
    }
}
</script>
<template lang="">
    <header>
       <a href="/" class="brand">
            <img :src="logo" alt="logoDc">
       </a>
        <nav>
            <ul>
                <li v-for="(item, index) in nav" :key="index">
                    <a :href="item.url" :class="item.active ? 'active' : ''">
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
</style>