<script>
    export default {
            props: {
                comics: Array,
            },
            jumbo: "./src/assets/img/jumbotron.jpg"
        
    
    }
</script>


<template lang="">
    <div class="jumbotron">
    </div>
    <div class="bg-black">
        <div class="container">
            <div class="current-button">CURRENT SERIES</div>
            <div class="row">
                <div class="col" v-for="(item, index) in comics" :key="index">
                    <div class="card-img">
                        <img :src="item.thumb" :alt="item.series">
                    </div>
                    <div class="title">
                        {{item.series}}
                    </div>
                </div>
            </div>
            <button class="load-button">LOAD MORE</button>
        </div>
    </div>
</template>


<style lang="scss">
    @use './src/styles/partials/_variables.scss' as *;
    @use './src/styles/partials/_mixins.scss' as *;

    
    .jumbotron{
        width: 100%;
        background-image: url('src/assets/img/jumbotron.jpg');
        background-size: cover;
        height: 350px;
    }

    .bg-black{
        background-color: rgba(28,28,28,255);
        text-align: center;

        .container{
            @include width70;
            position: relative;

            .current-button{
                position: absolute;
                top: 0;
                left: 0;
                transform: translateY(-50%);
                padding: 5px 10px;
                background-color: $blue;
                font-weight: 600;
                cursor: pointer;
                color: white;
            }

            .row{
                display: flex;
                flex-wrap: wrap;
                padding: 40px 0 0 0;


                .col{
                    width: calc(100% / 6);
                    margin: 10px 0;

                    .card-img{

                        img{
                            height: 150px;
                            width: 150px;
                        }
                    }

                    .title {
                        color: white;
                        font-size: 13px;
                        text-transform: uppercase ;
                    }
                }
            }

            .load-button{
                background-color: $blue;
                border: none;
                cursor: pointer;
                color: white;
                padding: 5px 30px;
                font-weight: 600;
                margin: 40px 0 20px 0;

                &:active, &:hover{
                    border: none;
                    background-color: #ffffffd5;
                    color: rgb(0, 0, 0);
                    transition: background-color, color, 2s;
                }
                
            }
        }
    }
</style>