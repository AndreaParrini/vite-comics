<script>
export default {
    name: 'AppHeader'
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
                    <li><a href="#">Characters</a></li>
                    <li><a href="#" class="active">Comics</a></li>
                    <li><a href="#">Movies</a></li>
                    <li><a href="#">Tv</a></li>
                    <li><a href="#">Games</a></li>
                    <li><a href="#">Collectibles</a></li>
                    <li><a href="#">Videos</a></li>
                    <li><a href="#">Fans</a></li>
                    <li><a href="#">News</a></li>
                    <li><a href="#">Shop</a></li>
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