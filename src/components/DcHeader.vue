<script>
export default {
    name: "DcHeader",
    data() {
        return {
            linkings: [
                {
                    name: 'characters',
                    url: '/',
                    current: 'false'
                },
                {
                    name: 'comics',
                    url: '/',
                    current: 'true'
                },
                {
                    name: 'movies',
                    url: '/',
                    current: 'false'
                },
                {
                    name: 'tv',
                    url: '/',
                    current: 'false'
                },
                {
                    name: 'games',
                    url: '/',
                    current: 'false'
                },
                {
                    name: 'collectibles',
                    url: '/',
                    current: 'false'
                },
                {
                    name: 'videos',
                    url: '/',
                    current: 'false'
                },
                {
                    name: 'fans',
                    url: '/',
                    current: 'false'
                },
                {
                    name: 'news',
                    url: '/',
                    current: 'false'
                },
                {
                    name: 'shop',
                    url: '/',
                    current: 'false'
                }
            ]
        }
    }
}
</script>

<template>
    <div class="backTotal">
        <header>
            <img src="../../public/img/dc-logo.png" alt="">
            <nav>
                <ul>
                    <li v-for="(element, index) in linkings" :key="index" :class="element.current ? 'active' : ''">
                        <a :href="element.url">{{ element.name }} </a>
                    </li>
                </ul>
            </nav>
        </header>
    </div>
</template>

<style scooped lang="scss" as *>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: sans-serif;
}

.backTotal {
    height: 100vh;
}

header {

    background-color: aquamarine;
    height: 10%;
    display: flex;
    justify-content: space-between;
    align-items: center;



    nav {

        ul {
            list-style: none;
            display: flex;
            justify-content: space-between;
            align-items: center;



            li {
                &.active a {
                    color: blue;
                }

                a {
                    text-decoration: none;
                    text-transform: uppercase;
                    font-size: 0.8rem;
                    margin: 0 1rem;
                    font-weight: bold;

                }

            }



        }
    }
}
</style>