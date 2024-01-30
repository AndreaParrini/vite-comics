<script>
export default {
    name: 'AppMain'
}
</script>

<template>
    <main>
        <section class="content">
            <div class="container">
                --&gt; Content goes here &lt;--
            </div>
        </section>
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

main .link {
    background-color: var(--dc-primary);
    padding: 3rem 0;

    & .container {
        display: flex;
    }

    & .col {
        display: flex;

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