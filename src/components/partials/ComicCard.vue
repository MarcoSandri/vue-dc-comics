<template>
    
    <div class="comicCard">
            <a href="#">
                <div class="comicImage">
                    <img :src="url" :alt="name">
                </div>
                <div class="text">
                    {{name}}
                </div>
            </a>
    </div>


</template>

<script>

export default {
    name : "ComicCard",
    props: {
        url : String,
        name : String
    }
}
</script>

<style scoped lang="scss">
    @import "../../assets/style/general.scss";
    @import "../../assets/style/colors.scss";

    .comicCard {
        margin: 2rem auto;
        width: 220px;

        a {
            text-decoration: none;

            .comicImage {
                height: 220px;
                width: 220px;

                img{
                    object-fit: cover;
                    object-position: top;

                    height: 100%;
                    width: 100%;
                }
            }

            .text {
                color: #fff;
                margin-top: 1rem;
                text-transform: uppercase;
            }
        }
    }
</style>