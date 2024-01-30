<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            linkMenu: [
                {
                    text: 'Characters',
                    link: '#',
                    isActive: false
                },
                {
                    text: 'Comics',
                    link: '#',
                    isActive: true
                },
                {
                    text: 'Movies',
                    link: '#',
                    isActive: false
                },
                {
                    text: 'Tv',
                    link: '#',
                    isActive: false
                },
                {
                    text: 'Games',
                    link: '#',
                    isActive: false
                },
                {
                    text: 'Collectibles',
                    link: '#',
                    isActive: false
                },
                {
                    text: 'Videos',
                    link: '#',
                    isActive: false
                },
                {
                    text: 'Characters',
                    link: '#',
                    isActive: false
                },
                {
                    text: 'Fans',
                    link: '#',
                    isActive: false
                },
                {
                    text: 'News',
                    link: '#',
                    isActive: false
                },
                {
                    text: 'Shop',
                    link: '#',
                    isActive: false
                }
            ]
        }
    }
}
</script>

<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="/img/dc-logo.png" alt="">
            </div>
            <nav>
                <ul class="main_menu">
                    <li v-for="link in      linkMenu     "><a :href='link.link' :class="{ active: link.isActive }">{{
                        link.text
                    }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>



<style scoped>
header {
    margin: 1rem 0;

    & .container {
        display: flex;
        justify-content: space-between;
    }

    & nav {
        display: flex;
        align-items: center;
    }

    & .main_menu {
        display: flex;
        align-items: center;

        & li {
            list-style: none;
            padding: 0 1rem;

            & a {
                text-decoration: none;
                text-transform: uppercase;
                color: var(--dc-dark);
                padding: 3.5rem 0;
                font-weight: 600;
                font-size: small;
            }

            & a.active {
                color: var(--dc-primary);
                border-bottom: 5px solid var(--dc-primary);
            }
        }
    }

}
</style>