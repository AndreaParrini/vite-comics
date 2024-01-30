<script>
export default {
    name: 'AppFooter'
}
</script>

<template>
    <footer>
        <section class="section_links">
            <div class="container">
                <div class="links">
                    <div class="col">
                        <h3>Dc Comics</h3>
                        <ul>
                            <li><a href="#">Characters</a></li>
                            <li><a href="#">Comics</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">TV</a></li>
                            <li><a href="#">Games</a></li>
                            <li><a href="#">Videos</a></li>
                            <li><a href="#">News</a></li>
                        </ul>
                        <h3>Shop</h3>
                        <ul>
                            <li><a href="#">Shop DC</a></li>
                            <li><a href="#">Shop DC Collectibles</a></li>
                        </ul>
                    </div>
                    <div class="col">
                        <h3>Dc</h3>
                        <ul>
                            <li><a href="#">Term Of Use</a></li>
                            <li><a href="#">Privacy policy (New)</a></li>
                            <li><a href="#">Ad Choices</a></li>
                            <li><a href="#">Advertising</a></li>
                            <li><a href="#">Jobs</a></li>
                            <li><a href="#">Subscriptions</a></li>
                            <li><a href="#">Talent Workshops</a></li>
                            <li><a href="#">CPSC Certificates</a></li>
                            <li><a href="#">Ratings</a></li>
                            <li><a href="#">Shop Help</a></li>
                            <li><a href="#">Contact Us</a></li>
                        </ul>
                    </div>
                    <div class="col">
                        <h3>Sites</h3>
                        <ul>
                            <li><a href="#">Dc</a></li>
                            <li><a href="#">MAD Magazine</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">DC Kids</a></li>
                            <li><a href="#">DC Universe</a></li>
                            <li><a href="#">DC Power Visa</a></li>
                        </ul>
                    </div>
                </div>
                <div class="thumb">
                    <img src="/img/dc-logo-bg.png" alt="">
                </div>
            </div>
        </section>

        <section class="section_follow">
            <div class="container">
                <div class="sign_up">
                    <div class="btn">
                        <a href="#">sign-up now!</a>
                    </div>
                </div>
                <div class="follow_us">
                    <h3>Follow Us</h3>
                    <ul class="footer_menu">
                        <li><a href="#"><img src="/img/footer-facebook.png" alt=""></a></li>
                        <li><a href="#"><img src="/img/footer-twitter.png" alt=""></a></li>
                        <li><a href="#"><img src="/img/footer-youtube.png" alt=""></a></li>
                        <li><a href="#"><img src="/img/footer-pinterest.png" alt=""></a></li>
                        <li><a href="#"><img src="/img/footer-periscope.png" alt=""></a></li>
                    </ul>
                </div>
            </div>

        </section>
    </footer>
</template>

<style scoped>
.section_links {
    background-image: url(/img/footer-bg.jpg);
    background-size: cover;

    & .container {
        display: flex;
        justify-content: space-between;
    }

    & .links {
        display: flex;
    }

    & img {
        height: 400px;
        overflow: hidden;
    }

    & h3 {
        text-transform: uppercase;
        color: var(--dc-light);
        margin-top: 1.5rem;
        margin-bottom: 1rem;
        font-size: larger;
        font-weight: 700;
    }

    & li {
        list-style: none;

        & a {
            text-decoration: none;
            color: var(--dc-gray);
            font-size: small;
            font-weight: 200;
        }
    }

    & img {
        height: 600px;
        margin-top: -100px;
        margin-bottom: -100px;
    }

}


.section_follow {
    background-color: var(--dc-footer);
    position: relative;
    padding: 2rem;

    & .container {
        display: flex;
        justify-content: space-between;
    }

    & .btn {
        padding: 1rem;
        border: 2px solid var(--dc-primary);

        & a {
            text-transform: uppercase;
            color: var(--dc-light);
            text-decoration: none;
        }
    }

    .follow_us {
        display: flex;
        align-items: center;

        & h3 {
            color: var(--dc-primary);
            text-transform: uppercase;
            font-size: larger;
            font-weight: 700;
            margin-right: 1rem;
        }
    }

    & .footer_menu {
        display: flex;

        & li {
            list-style: none;
            padding: 0.5rem;
        }
    }

}
</style>