<script>

export default {
    name: "DigitalDetails",
    props: ['digitalElement']
}
</script>

<template>
    <div class="mainDig">
        <img :src="digitalElement.src" alt="">
        <span>{{ digitalElement.name }}</span>
    </div>
</template>

<script scoped lang="scss">
</script>