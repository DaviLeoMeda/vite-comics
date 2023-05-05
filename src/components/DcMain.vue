<script>
export default {
    name: "DcMain",
    data() {
        return {
            mainImg: [
                {
                    name: 'digital comics',
                    src: '../../public/img/buy-comics-digital-comics.png'
                },
                {
                    name: 'dc merchandise',
                    src: '../../public/img/buy-comics-merchandise.png'
                },
                {
                    name: 'subscriptions',
                    src: '../../public/img/buy-comics-subscriptions.png'
                },
                {
                    name: 'comic shop locator',
                    src: '../../public/img/buy-comics-shop-locator.png'
                },
                {
                    name: 'dc power visa',
                    src: '../../public/img/buy-dc-power-visa.svg'
                },


            ]

        }
    }


}
</script>

<template>
    <main>

        <div class="firstMain">
            Qui ci andranno i fumetti
        </div>

        <div class="secondMain">

        </div>

    </main>
</template>

<style lang="scss" scoped>
main {

    .firstMain {
        background-color: rgb(15, 15, 15);
        height: 100px;
        color: white;
    }

    .secondMain {
        background-color: rgb(74, 74, 238);
        height: 130px;
    }

}
</style>