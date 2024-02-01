<script>
export default {
    name: 'AppReferalLink'
}
</script>

<template>
    <section class="link">
        <div class="container">
            <div class="col">
                <img src="/img/buy-comics-digital-comics.png" alt="">
                <a href="#">Digital Comics</a>
            </div>
            <div class="col">
                <img src="/img/buy-comics-merchandise.png" alt="">
                <a href="#">Dc Merchandise</a>
            </div>
            <div class="col">
                <img src="/img/buy-comics-subscriptions.png" alt="">
                <a href="#">Subscription</a>
            </div>
            <div class="col">
                <img src="/img/buy-comics-shop-locator.png" alt="">
                <a href="#">Comic Shop locator</a>
            </div>
            <div class="col">
                <img src="/img/buy-dc-power-visa.svg" alt="">
                <a href="#">Dc Power Visa</a>
            </div>
        </div>
    </section>
</template>


<style scoped>
.link {
    background-color: var(--dc-primary);
    padding: 3rem 0;
    position: relative;

    & .container {
        display: flex;
    }

    & .col {
        display: flex;
        justify-content: center;

        & img {
            max-height: 4rem;
            max-width: 4rem;
        }

        & a {
            text-decoration: none;
            color: var(--dc-light);
            display: flex;
            align-items: center;
            margin-left: 0.5rem;
            font-weight: 500;
            font-size: 0.9rem;
            text-transform: uppercase;
        }
    }
}
</style>