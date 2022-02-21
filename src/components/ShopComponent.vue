<template>
    <section class="shop">
        <div class="container">
            <ul>
                <li><a href="#"><img src="../assets/img/buy-comics-digital-comics.png">DIGITAL COMICS</a></li>
                <li><a href="#"><img src="../assets/img/buy-comics-merchandise.png">DC MERCHANDISE</a></li>
                <li><a href="#"><img src="../assets/img/buy-comics-subscriptions.png">SUBSCRIPTION</a></li>
                <li><a href="#"><img src="../assets/img/buy-comics-shop-locator.png">COMIC SHOP LOCATOR</a></li>
                <li><a href="#"><img src="../assets/img/buy-dc-power-visa.svg" class="svg">DC POWER VISA</a></li>
            </ul>
        </div>
    </section>
</template>

<script>
export default {
    name: 'ShopComponent'
}
</script>

<style scoped lang="scss">
    @import '../assets/style/general.scss';
    @import '../assets/style/colors.scss';

    .shop {
        background-color: $secondary;
    }

    ul {
        display: flex;
        justify-content: space-around;

        li {
            a {
                display: flex;
                align-items: center;
                color: #fff;

                img {
                    margin-right: 1rem;
                    height: 4rem;
    
                    &.svg {
                        transform: scale(70%)
                    }
                }
            }
        }
    }

</style>