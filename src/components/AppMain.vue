<script>
import AppReferalLink from './AppReferalLink.vue';

export default {
    name: 'AppMain',
    components: {
        AppReferalLink
    }
}
</script>

<template>
    <main>
        <section class="content">
            <div class="container">
                --&gt; Content goes here &lt;--
            </div>
        </section>
        <AppReferalLink></AppReferalLink>
    </main>
</template>


<style scoped>
main .content {
    background-color: var(--dc-dark);
    color: var(--dc-light);
    font-size: 1.5rem;
    font-weight: 700;
    padding: 3rem 0;
}
</style>