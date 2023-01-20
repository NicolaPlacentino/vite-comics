<script>
export default {
    name: 'AppFooter',

}
</script>

<template>
    <div class="p-absolute">
        <div class="jumbo-bg">
            <div class="container">
                <div class="d-flex">
                    <div class="col">
                        <h3>DC Comics</h3>
                        <ul>
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Movies</li>
                            <li>TV</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ul>
                        <h3>Shop</h3>
                        <ul>
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li>
                        </ul>
                    </div>
                    <div class="col">
                        <h3>DC</h3>
                        <ul>
                            <li>Terms of Use</li>
                            <li>Privacy policy (New)</li>
                            <li>Ad Choices</li>
                            <li>Advertising</li>
                            <li>Jobs</li>
                            <li>Subcriptions</li>
                            <li>Talent Workshops</li>
                            <li>CPSC Certificates</li>
                            <li>Ratings</li>
                            <li>Shop Help</li>
                            <li>Contact Us</li>
                        </ul>
                    </div>
                    <div class="col">
                        <h3>Sites</h3>
                        <ul>
                            <li>DC</li>
                            <li>MAD Magazine</li>
                            <li>DC Kids</li>
                            <li>DC Universe</li>
                            <li>DC Power Visa</li>
                        </ul>
                    </div>
                </div>
                <div>
                    <figure>
                        <img src="../assets/img/dc-logo-bg.png" alt="DC">
                    </figure>
                </div>
            </div>
        </div>
        <div class="gray-bg">
            <div class="container">
                <button>SIGN-UP NOW!</button>

                <div>
                    <a href="#">FOLLOW US</a>
                    <ul>
                        <li><img src="../assets/img/footer-facebook.png" alt="social"></li>
                        <li><img src="../assets/img/footer-twitter.png" alt="social"></li>
                        <li><img src="../assets/img/footer-youtube.png" alt="social"></li>
                        <li><img src="../assets/img/footer-pinterest.png" alt="social"></li>
                        <li><img src="../assets/img/footer-periscope.png" alt="social"></li>

                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../assets/scss/variables' as *;

.p-absolute {
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;


    .jumbo-bg {
        background-image: url(../assets/img/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;

        height: 300px;

        color: white;

        .container {
            display: flex;
            justify-content: space-between;

            height: 100%;

            .col {
                padding: 40px 20px;

                h3 {
                    font-family: $font-condensed;
                    text-transform: uppercase;
                    margin-bottom: 5px;
                }

                ul {
                    list-style-type: none;

                    margin-bottom: 10px;

                    li {
                        font-size: 12px;
                        color: gray;
                    }
                }
            }

            figure {
                width: 450px;
                height: 100%;

                overflow: hidden;


                img {
                    transform: translateY(-17%);
                    width: 100%;
                    height: auto;
                }
            }
        }
    }

    .gray-bg {
        background-color: rgb(60, 60, 60);
        padding: 30px 0;

        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;

            button {
                padding: 10px;
                font-size: 20px;

                color: white;
                background-color: rgba(#000000, 0);

                border: 3px solid dodgerblue;

                cursor: pointer;
            }

            div {
                display: flex;
                align-items: center;

                a {
                    color: dodgerblue;
                    text-decoration: none;

                    font-size: 25px;
                    font-family: $font-condensed;
                    font-weight: bold;

                    margin-right: 10px;
                }

                ul {
                    list-style-type: none;

                    display: flex;

                    li {
                        margin: 0 10px;

                        img {
                            height: 40px;
                            width: auto;
                        }
                    }
                }
            }
        }
    }
}
</style>