<script>
export default {
    props: {
        thumb: String,
        series: String
    }
}
</script>
<template>
    <div>
        <div class="card col-3">
            <img :src="thumb" alt="action-comics">
            <div class="series">{{ series }}</div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
    .card {
        background-color: black;
        color: white;
        display: flex;
        flex-wrap: wrap;
        img {
            height: 200px;
            width: 150px;
        }
    }
</style>