<script>
export default {
    name: 'Button',
    props: {
        text: String
    }
}
</script>

<template>
    <button>{{ text }}</button>
</template>

<style lang="scss" scoped>
@use '../assets/scss/variables' as *;

button {
    background-color: dodgerblue;
    color: white;
    font-family: $font-condensed;
    font-weight: bold;
    font-size: 16px;

    padding: 5px 10px;

    text-transform: uppercase;

    cursor: pointer;

    margin: 20px 0;
}
</style>