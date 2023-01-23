<script>
import Button from './MainSecondaryComponents/Button.vue'
import Card from './MainSecondaryComponents/Card.vue'
export default {
    name: 'AppMain',
    components: { Button, Card },
    data() {
        return {
            ButtonText: 'Load more'
        }
    },
    props: {
        comics: Array
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
                <Card v-for="comic in comics"></Card>
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

    .card-section {
        display: flex;
        flex-wrap: wrap;
    }

}

.text-center {
    text-align: center;
}
</style>