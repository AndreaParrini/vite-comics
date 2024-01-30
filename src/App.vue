<script >
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'

export default {
  name: 'App',
  components: {
    AppHeader,
    AppMain
  }
}
</script>

<template>
  <AppHeader></AppHeader>
  <AppMain></AppMain>

  <footer>
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
        <div class="col"></div>
        <div class="col"></div>
      </div>
      <div class="thumb">
        <img src="/img/dc-logo-bg.png" alt="">
      </div>
    </div>
  </footer>
</template>

<style>
footer {
  background-image: url(/img/footer-bg.jpg);
  background-size: cover;

  & .container {
    display: flex;
    justify-content: space-between;
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
      color: var(--dc-light);
      font-size: small;
      font-weight: 200;
    }
  }

}

/* .thumb {
  width: 325px;
  height: 150px;
  overflow: hidden;
}

.thumb>img {
  height: 200px;
  width: 325px;
  margin-top: -30px;
} */
</style>
