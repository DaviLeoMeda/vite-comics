<script>

import DigitalDetails from './DigitalDetails.vue'

export default {
    name: "DcMain",
    components: {
        DigitalDetails
    },
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

        </div>

        <div class="backSide">
            <div class="secondMain">
                <DigitalDetails v-for="( elem, index ) in mainImg" :key="index" :digitalElement="elem" />
            </div>
        </div>

    </main>
</template>

<style lang="scss" scoped>
main {

    .firstMain {
        // background-color: rgb(15, 15, 15);
        height: 300px;
        background-image: url(../../public/img/jumbotron.jpg);
        background-repeat: no-repeat;
        background-size: cover;



    }

    .backSide {

        background-color: rgb(74, 74, 238);

        .secondMain {

            width: 80%;
            margin: 0 auto;
            display: flex;
            align-items: center;
            justify-content: space-around;


            .mainDig {
                display: flex;
                align-items: center;
                padding: 100px 10px;
                text-transform: uppercase;
                color: #fff;

            }
        }
    }


}
</style>