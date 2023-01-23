<script>
export default {
    name: 'Card',
    props: {
        comic: Object
    }
}
</script>

<template>
    <div class="card">
        <figure>
            <img :src="comic.thumb" :alt="comic.series">
            <figcaption>{{ comic.series }}</figcaption>
        </figure>
    </div>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/variables' as *;

.card {
    width: calc(100% / 6);
    padding: 10px;

    figure {

        img {
            width: 100%;
            height: 180px;
            object-fit: cover;
            object-position: top;
        }

        figcaption {
            color: white;
            font-size: 16px;
            text-transform: uppercase;

            margin: 10px 0;
        }
    }
}
</style>