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
            <div class="row">
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
        </div>
    </div>
    <div class="bg-grey">
        <div class="last-container">
            <button>
                <a href="#"> SIGN-UP NOW!</a>
            </button>
            <div class="icons">
                <h2>FOLLOW US</h2>
                <div>
                    <i class="fa-brands fa-facebook-f"></i>
                </div>
                <div>
                    <i class="fa-brands fa-twitter"></i>  
                </div>
                <div>
                    <i class="fa-brands fa-youtube"></i>
                </div>
                <div>
                    <i class="fa-brands fa-pinterest-p"></i>
                </div>
                <div>
                    <i class="fa-brands fa-periscope"></i>
                </div>
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
            background-image: url('src/assets/img/dc-logo-bg.png');
            background-repeat: no-repeat;
            background-position: right center;

            .row{
                display: flex;
                width: 40%;
                padding: 30px 0;


                .col{
                    display: flex;
                    flex-direction: column;
                    padding: 0 15px;
                    font-size: 13px;
                    color: white;


                    a{
                        text-decoration: none;
                        color: grey;
                        &:focus, &:active{
                            outline: none
                        }
                    }
                }
            }
        }
    };

    .bg-grey{
        background-color: rgba(48,48,48,255);

        .last-container{
            @include width70;
            @include center;


            button{
                border: 2px solid $blue;
                background-color: rgba(48,48,48,255);
                margin: 20px 15px;
                padding: 10px ;

                a{
                    text-decoration: none;
                    color: white;
                    font-weight: 600;

                    &:focus, &:active{
                        outline: none;
                    }
                }
            }

            .icons{
                display: flex;
                align-items: center;

                h2{
                    color: $blue;
                    font-size: 20px;
                    margin-right: 20px;

                }

                div{
                    background-color: grey;
                    width: 25px;
                    height: 25px;
                    text-align: center;
                    margin: 0 10px;
                    border-radius: 20px;

                    i{
                        padding: 2px;
                        color:rgba(48,48,48,255) ;
                    }
                }
            }
        }
    }
</style>