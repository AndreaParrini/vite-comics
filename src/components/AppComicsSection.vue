<script>
import AppCardItem from './AppCardItem.vue';

export default {
    name: 'AppComicsSection',
    data() {
        return {
            items: [
                {
                    "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book",
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book",
                },
                {
                    "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel",
                },
                {
                    "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book",
                },
                {

                    "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",

                    "price": "$3.99",

                    "series": "Batman",

                    "type": "comic book",

                },

                {

                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",

                    "price": "$2.99",

                    "series": "Batman Beyond",

                    "type": "comic book",

                },

                {

                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",

                    "price": "$3.99",

                    "series": "Batman/Superman",

                    "type": "comic book",

                },

                {

                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",

                    "price": "$4.99",

                    "series": "Batman/Superman Annual",

                    "type": "comic book",

                },

                {

                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",

                    "price": "$5.99",

                    "series": "Batman: The Joker War Zone",

                    "type": "comic book",

                },

                {

                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",

                    "price": "$6.99",

                    "series": "Batman: Three Jokers",

                    "type": "comic book",

                },

                {

                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",

                    "price": "$4.99",

                    "series": "Batman: White Knight Presents: Harley Quinn",

                    "type": "comic book",

                },

                {

                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",

                    "price": "$16.99",

                    "series": "Catwoman",

                    "type": "graphic novel",

                },

            ]
        }
    },
    components: {
        AppCardItem
    }
}
</script>

<template>
    <section class="content">
        <div class="container">
            <h4 class="title box">Current Series</h4>
            <div class="row">
                <AppCardItem :thumb="item.thumb" :series="item.series" v-for=" item  in  items "></AppCardItem>
                <button class="box">Load more</button>
            </div>
        </div>
    </section>
</template>



<style scoped>
.content {
    background-color: var(--dc-dark);
    color: var(--dc-light);
    font-size: 1.5rem;
    font-weight: 700;
    padding: 3rem 0;

    & .box {
        background-color: var(--dc-primary);
        color: var(--dc-light);
        text-transform: uppercase;
        padding: 1rem 1rem;
    }

    & .title {
        width: 165px;
        font-size: medium;
        margin-top: -4.5rem;
        margin-bottom: 2rem;
        margin-left: 1rem;
    }

    & button {
        margin: auto;
        font-size: small;
        border-style: none;
    }
}
</style>