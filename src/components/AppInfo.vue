
<script>
export default {
    data() {
        return {
            items: [
                {
                    img: "src/assets/img/buy-comics-digital-comics.png",
                    item: "DIGITAL COMICS",
                    url: "#"
                },
                {
                    img: "src/assets/img/buy-comics-merchandise.png",
                    item: "DC MERCHANDISE",
                    url: "#"
                },
                {
                    img: "src/assets/img/buy-comics-subscriptions.png",
                    item: "SUBSCRIPTIONS",
                    url: "#"
                },
                {
                    img: "src/assets/img/buy-comics-shop-locator.png",
                    item: "COMIC SHOP LOCATOR",
                    url: "#"
                },
                {
                    img: "src/assets/img/buy-dc-power-visa.svg",
                    item: "DC POWER VISA",
                    url: "#"
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
                <li v-for="(oggetto, index) in items" :key="index">
                    <div class="img-container">
                        <img :src="oggetto.img" alt="logoItem">
                    </div>
                    <a :href="oggetto.url" class="link">
                        {{oggetto.item}}
                    </a>
                    
                </li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss">
    @use './src/styles/partials/_variables.scss' as *;
    @use './src/styles/partials/_mixins.scss' as *;

    .bg-blue{
        background-color: $blue;

        .container{
            @include width70;

            ul{
                list-style-type: none;
                @include center;
                padding: 30px;

                li{
                    @include center;

                    .img-container{
                        width: 80px;
                        height: 80px;
                        display: flex;
                        align-items: center;


                        img{
                            width: 90%;
                            height: 100%;
                            padding: 10px;
                        }
                    }

                    .link{
                        text-decoration: none;
                        color: white;
                    }

                    
                }
            }
        }
    }
</style>