<script>
import AppJumbotron from './AppJumbotron.vue';
import AppComicsSection from './AppComicsSection.vue';
import AppReferalLink from './AppReferalLink.vue';

export default {
    name: 'AppMain',
    components: {
        AppReferalLink,
        AppComicsSection,
        AppJumbotron
    }
}
</script>

<template>
    <main>
        <AppJumbotron></AppJumbotron>
        <AppComicsSection></AppComicsSection>
        <AppReferalLink></AppReferalLink>
    </main>
</template>


<style scoped></style>