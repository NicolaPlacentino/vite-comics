<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            navLinks: [
                {
                    text: 'Characters',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Comics',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Movies',
                    url: '#',
                    current: false,
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Games',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Collectibles',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Videos',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Fans',
                    url: '#',
                    current: false,
                },
                {
                    text: 'News',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Shop',
                    url: '#',
                    current: false,
                },
            ],
        }
    },
}
</script>

<template>
    <header>
        <div class="container">
            <figure>
                <a href="#">
                    <img src="../assets/img/dc-logo.png" alt="DC">
                </a>
            </figure>
            <ul>
                <li v-for="link in navLinks" v-bind:key="link.text" :class="{ 'active': link.current }">
                    <a :href="link.url">
                        {{ link.text }}
                    </a>
                </li>
            </ul>
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use '../assets/scss/variables' as *;


header {
    height: 150px;

    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 100%;

        figure {
            height: 90px;

            a {
                height: 100%;

                img {
                    height: 100%;
                    width: auto;
                }
            }
        }

        ul {
            display: flex;
            list-style-type: none;
            height: 100%;


            li {
                padding: 0 12px;
                height: 100%;

                display: flex;
                align-items: center;


                a {
                    text-decoration: none;
                    color: black;
                    font-size: 22px;
                    font-family: $font-condensed;
                    font-weight: bold;
                }

                &.active {
                    border-bottom: 5px solid dodgerblue;

                    a {
                        color: dodgerblue;
                    }
                }
            }
        }
    }
}
</style>