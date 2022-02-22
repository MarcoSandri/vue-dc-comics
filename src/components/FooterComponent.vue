<template>
    <footer>
        <section class="links">
            <div class="container">
                <div class="lists">
                    <ul>
                        <li><h2>DC COMICS</h2></li>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Comics</a></li>
                        <li><a href="#">Movies</a></li>
                        <li><a href="#">TV</a></li>
                        <li><a href="#">Games</a></li>
                        <li><a href="#">Videos</a></li>
                        <li><a href="#">News</a></li>
                    </ul>

                    
                    <ul>
                        <li><h2>SHOP</h2></li>
                        <li><a href="#">Shop DC</a></li>
                        <li><a href="#">Shop DC Collectibles</a></li>
                    </ul>

                    <ul>
                        <li><h2>DC</h2></li>
                        <li><a href="#">Terms Of Use</a></li>
                        <li><a href="#">Privacy Police (New)</a></li>
                        <li><a href="#">Ad Choice</a></li>
                        <li><a href="#">Advertising</a></li>
                        <li><a href="#">Jobs</a></li>
                        <li><a href="#">Subscriptions</a></li>
                        <li><a href="#">Talent Workshops</a></li>
                        <li><a href="#">CPSC Certificates</a></li>
                        <li><a href="#">Ratings</a></li>
                        <li><a href="#">Shop Help</a></li>
                        <li><a href="#">Contact Us</a></li>
                    </ul>

                    <ul>
                        <li><h2>SITES</h2></li>
                        <li><a href="#">DC</a></li>
                        <li><a href="#">MAD Magazine</a></li>
                        <li><a href="#">DC Kids</a></li>
                        <li><a href="#">DC Universe</a></li>
                        <li><a href="#">DC Power Visa</a></li>
                    </ul>
                </div>
                <div class="footerLogo">
                    <img src="../assets/img/dc-logo-bg.png">
                </div>
            </div>
        </section>

        <section class="follow">
            <div class="container">
                <button>SIGN-UP NOW!</button>
                <div class="social">
                    <h1>FOLLOW US</h1>
                    <ul>
                        <li v-for="(social, index) in socials" :key="index"><a href="#"><img :src="require('../assets/img/'+ social.url)"></a></li>
                    </ul>
                </div>
            </div>
        </section>
    </footer>
</template>

<script>
    export default {
        name : "FooterComponent",
        data() {
            return {
            socials : [
                {   
                    name: "facebook",
                    url : "footer-facebook.png"
                },
                {   
                    name: "twitter",
                    url : "footer-twitter.png"
                },
                {   
                    name: "youtube",
                    url : "footer-youtube.png"
                },
                {   
                    name: "pinterest",
                    url : "footer-pinterest.png"
                },
                {   
                    name: "periscope",
                    url : "footer-periscope.png"
                }
            ]
            }
        }
    }
</script>

<style lang="scss" scoped>
    @import '../assets/style/general.scss';
    @import '../assets/style/colors.scss';

    footer {
        display: flex;
        flex-direction: column;
    }

    .links {
        background-image: url(../assets/img/footer-bg.jpg);
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
        overflow: hidden;

        .container {
            display: flex;
            justify-content: space-between;
            position: relative;

            .lists {
                color: #fff;
                display: flex;
                flex-direction: column;
                flex-wrap: wrap;
                height: 350px;
                
                ul {
                    margin: 0 1rem;
                    li {
                        padding: 0.1rem 0;
                        
                        h2 {
                            padding: 1rem 0;
                        }
    
                        a {
                            color: gray;
                            font-size: 0.8rem;
                        }
                    }
                }
            }

            .footerLogo {
                position: absolute;
                right: 0;
                top: 50%;
                transform: translate(0, -50%)
            }
        }
        
    }

    .follow {
        background-color: $footer;

        .container {
            display: flex;
            justify-content: space-between;

            button{
                background-color: transparent;
                border: 2px solid $secondary;
                color: #fff;
                padding: 0.75rem;
                font-size: 1.25rem;
            }

            .social {
                display: flex;
                align-items: center;

                h1 {
                    color: $secondary;
                    margin: 0 0.75rem;
                }

                ul {
                    display: flex;

                    li{
                        margin: 0 0.75rem;
                    }
                }
            }
        }
    }
</style>