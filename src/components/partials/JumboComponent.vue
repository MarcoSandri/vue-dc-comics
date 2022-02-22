<template>
    <div class="jumbotron">
        <img src="../../assets/img/jumbotron.jpg" alt="">
    </div>
</template>

<script>

export default {
    name : "JumboComponent"
}
</script>

<style scoped lang="scss">
    @import "../../assets/style/general.scss";

    .jumbotron {
        height: 400px;
        
        img{
            object-fit: cover;
            object-position: top;

            height: 100%;
            width: 100%;
        }
    }
</style>