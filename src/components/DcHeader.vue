<script>
export default {
    name: "DcHeader",
    data() {
        return {
            linkings: [
                {
                    name: 'characters',
                    url: '/',
                    current: false
                },
                {
                    name: 'comics',
                    url: '/',
                    current: true
                },
                {
                    name: 'movies',
                    url: '/',
                    current: false
                },
                {
                    name: 'tv',
                    url: '/',
                    current: false
                },
                {
                    name: 'games',
                    url: '/',
                    current: false
                },
                {
                    name: 'collectibles',
                    url: '/',
                    current: false
                },
                {
                    name: 'videos',
                    url: '/',
                    current: false
                },
                {
                    name: 'fans',
                    url: '/',
                    current: false
                },
                {
                    name: 'news',
                    url: '/',
                    current: false
                },
                {
                    name: 'shop',
                    url: '/',
                    current: false
                }
            ]
        }
    }
}
</script>

<template>
    <header>
        <div class="container">
            <img src="../../public/img/dc-logo.png" alt="">
            <nav>
                <ul>
                    <li v-for="(element, index) in linkings" :key="index" :class="element.current ? 'active' : ''">
                        <a :href="element.url">{{ element.name }} </a>
                    </li>
                </ul>
            </nav>
        </div>

    </header>
</template>

<style scooped lang="scss" as *>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: sans-serif;
}

.container {
    width: 80%;
    margin: 0 auto;

}


header {

    div {

        height: 100px;
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
                    line-height: 100px;

                    &.active {
                        border-bottom: 5px solid blue;
                    }

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


}
</style>