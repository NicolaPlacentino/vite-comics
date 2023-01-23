<script>
export default {
    name: 'Card',
    props: {

    }
}
</script>

<template>
    <div class="card">
        <figure>
            <img src='https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq'
                alt="alt">
            <figcaption>Catwoman</figcaption>
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
            font-size: 18px;
            text-transform: uppercase;

            margin: 10px 0;
        }
    }
}
</style>