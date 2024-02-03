
<script>
export default {
    name: 'AppCardItem',
    props: {
        thumb: String,
        series: String
    }
}
</script>

<template>
    <div class="col-2">
        <div class="card">
            <img :src="thumb" alt="">
            <h6>{{ series }}</h6>
        </div>
    </div>
</template>


<style scoped>
img {
    max-width: 100%;
    aspect-ratio: 1;
    object-fit: cover;
    object-position: top;
}

h6 {
    text-transform: uppercase;
    font-size: small;
}
</style>