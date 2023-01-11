<script>
export default {
    data() {
        return {
            imgLogo: "src/assets/img/dc-logo-bg.png"
        }
    } 
}
</script>

<template lang="">
    <div class="bg">
        <div class="container">
            <div class="col1">
                <div class="col">
                    <h2>DC COMICS</h2>
                    <a href="">Characters</a>
                    <a href="">Comics</a>
                    <a href="">Movies</a>
                    <a href="">TV</a>
                    <a href="">Games</a>
                    <a href="">Videos</a>
                    <a href="">News</a>
                    <h2>SHOP</h2>
                    <a href="">Shop DC</a>
                    <a href="">Shop DC Collectibles</a>
                </div>
                <div class="col">
                    <h2>DC</h2>
                    <a href="">Terms Of Use</a>
                    <a href="">Privacy Policy (New)</a>
                    <a href="">Ad Choices</a>
                    <a href="">Advertising</a>
                    <a href="">Jobs</a>
                    <a href="">Subscriptions</a>
                    <a href="">Talent Workshops</a>
                    <a href="">CPSC Certificates</a>
                    <a href="">Ratings</a>
                    <a href="">Shop Help</a>
                    <a href="">Contact Us</a>
                </div>
                <div class="col">
                    <h2>SITES</h2>
                    <a href="">DC</a>
                    <a href="">MAD Magazine</a>
                    <a href="">DC Kids</a>
                    <a href="">DC Universe </a>
                    <a href="">DC Power Visa</a>
                </div>
            </div>
            <div class="img-container col2">
                <img :src="imgLogo" alt="">
            </div>
        </div>
    </div>
</template>

<style lang="scss">
    @use './src/styles/partials/_variables.scss' as *;
    @use './src/styles/partials/_mixins.scss' as *;

    .bg{
        background-image: url('src/assets/img/footer-bg.jpg');

        .container{
            @include width70;
            @include center;
        }
    }
</style>