<script>
export default {
    name: 'AppMain',

}
</script>

<template>
    <div>
        <span>Content goes here</span>
    </div>
</template>

<style lang="scss" scoped>
div {
    background-color: rgb(25, 25, 25);

    display: flex;
    justify-content: center;
    align-items: center;

    height: calc(100vh - 150px - 400px);

    span {
        color: white;
        font-size: 30px;
    }
}
</style>