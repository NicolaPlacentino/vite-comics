<script>
import Button from './Button.vue'
export default {
    name: 'AppMain',
    components: { Button },
    data() {
        return {
            ButtonText: 'Load more'
        }
    }
}
</script>

<template>
    <div>
        <div class="jumbo">
            <img src="../assets/img/jumbotron.jpg" alt="jumbotron">
        </div>
        <div class="container">
            <h2>Current series</h2>
            <div class="card-section">
                <div class="card">
                    <figure>
                        <img src='https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq'
                            alt="alt">

                        <figcaption>Catwoman</figcaption>

                    </figure>

                </div>
            </div>
            <div class="text-center">
                <Button :text="ButtonText"></Button>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../assets/scss/variables' as *;

div {
    background-color: rgb(25, 25, 25);

    .jumbo {
        overflow: hidden;

        height: 350px;

        img {
            width: 100%;
        }
    }

    h2 {
        background-color: dodgerblue;
        color: white;
        font-family: $font-condensed;
        font-weight: bold;

        display: inline-block;

        padding: 5px 10px;

        text-transform: uppercase;

        transform: translateY(-50%);
    }

    .card {
        width: calc(100% / 6);
        padding: 10px;

        figure {
            overflow: hidden;

            img {
                width: 100%;
                height: 180px;

                object-fit: cover;
                object-position: top;
            }

            figcaption {
                color: white;
                font-size: 18px;

                text-transform: uppercase;

                margin: 10px 0;
            }
        }
    }
}

.text-center {
    text-align: center;
}
</style>