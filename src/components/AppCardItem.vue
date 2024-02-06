
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
.card:hover {
    transform: scale(1.1);

    cursor: pointer;
}

img {
    max-width: 100%;
    aspect-ratio: 1;
    object-fit: cover;
    object-position: top;

    &:hover {
        filter: drop-shadow(0 0 5px var(--dc-light));
    }
}

h6 {
    text-transform: uppercase;
    font-size: small;
}
</style>