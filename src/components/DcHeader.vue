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
                    current: 'false'
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
    <header>
        <img src="../../public/img/dc-logo.png" alt="">
    </header>
    <nav>
        <ul>
            <li v-for="(element, index) in linkings" :key="index">
                <a :class="element.current ? 'active' : '' '" :href="element.url">{{ element.name }}</a>
            </li>
        </ul>
    </nav>
</template>

<style></style>