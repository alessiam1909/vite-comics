
<script>
export default {
    data() {
        return {
            items: [
                {
                    img: "src/assets/img/buy-comics-digital-comics.png",
                    item: "DIGITAL COMICS"
                },
                {
                    img: "src/assets/img/buy-comics-digital-merchandise.png",
                    item: "DC MERCHANDISE"
                },
                {
                    img: "src/assets/img/buy-comics-digital-subscriptions.png",
                    item: "SUBSCRIPTIONS"
                },
                {
                    img: "src/assets/img/buy-comics-digital-shop-locator.png",
                    item: "COMIC SHOP LOCATOR"
                },
                {
                    img: "src/assets/img/buy-dc-power-visa.png",
                    item: "DC POWER VISA"
                },
        
            ]
        }
    } 
}
</script>

<template lang="">
    <div class="bg-blue">
        <div class="container">
            <ul>
                <li v-for="(item, index) in items" :key="index">
                    <img :src="items.img" alt="">
                    <a href=""></a>
                </li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss">
    @use './src/styles/partials/_variables.scss' as *;
    @use './src/styles/partials/_mixins.scss' as *;
</style>