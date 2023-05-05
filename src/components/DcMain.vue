<script>
export default {
    name: "DcMain",
    data() {
        return {
            mainImg: [
                {
                    name: 'digital comics',
                    src: ''
                }
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