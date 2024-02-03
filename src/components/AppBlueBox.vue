<script>
export default {
    name: 'AppBlueBox',
    props: {
        text: String
    }
}
</script>

<template>
    <div class="box">
        <h4>{{ text }}</h4>
    </div>
</template>



<style scoped>
.box {
    background-color: var(--dc-primary);
    color: var(--dc-light);
    padding: 0.5rem 1rem;
    text-transform: uppercase;
}
</style>