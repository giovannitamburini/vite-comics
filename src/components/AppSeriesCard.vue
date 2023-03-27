<script>

export default {
    data() {
        return {

        }
    },

    props: {
        imgCard: String,
        titleCard: String,
    }
}

</script>

<template>
    <div class="card">
        <div class="card-img">
            <img :src="imgCard" alt="">
        </div>
        <div class="series">{{ titleCard }}</div>
    </div>
</template>

<style lang="scss" scoped>
.card {
    width: 165px;
    padding: 10px;
    color: white;
    text-transform: uppercase;

    .card-img {
        width: 100%;
        height: 165px - (10px * 2);
        overflow-y: hidden;


        img {
            width: 100%;
        }
    }

    .series {
        padding: 1em 0;
        word-wrap: break-word;
    }
}
</style>