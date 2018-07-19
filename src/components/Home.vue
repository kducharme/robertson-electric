<template>
  <div class="home">
    <Nav />
    <div class="home__hero">
      <h1>{{ msg }}</h1>
      <p>{{ sub }}</p>
    </div>
    <div class="home__services">
      <h3>Our services</h3>
      <div class="home__services--cards">
        <div class="card">
          <h5>Service name here</h5>
          <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium.</p>
        </div>
        <div class="card">
          <h5>Service name here</h5>
          <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium.</p>
        </div>
        <div class="card">
          <h5>Service name here</h5>
          <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium.</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Nav from "./Nav.vue";

export default {
  name: "Home",
  components: {
    Nav
  },
  data() {
    return {
      msg: "Quality, transparent electrical services.",
      sub:
        "At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium voluptatum deleniti atque corrupti quos dolores et quas molestias excepturi."
    };
  }
};
</script>

<style lang='scss'>
.home {
  background-image: url("../img/hero3.jpg");
  background-size: 100vw;
  width: 100vw;
  height: 75vh;
  .home__hero {
    display: flex;
    flex-direction: column;
    justify-content: center;
    height: calc(75vh);
    top: 0;
    margin-top: -60px;
    background: rgba(0, 0, 0, 0.45);
    padding: 0 80px;
    line-height: 1.7;
    h1 {
      font-family: 'Merriweather';
      width: 68vw;
      font-size: 38px;
      color: white;
      margin-bottom: 16px;
    }
    p {
      width: 68vw;
      color: white;
      font-size: 18px;
      font-weight: 400;
    }
  }
  .home__services {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-top: 60px;
    padding: 0 80px;
    h3 {
      font-size: 22px;
      font-weight: 600;
      margin-bottom: 32px;
    }
    .home__services--cards {
      display: flex;
      justify-content: space-between;
      .card {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        border: 1px solid rgb(207, 207, 207);
        height: 200px;
        text-align: center;
        line-height: 1.7;
        padding: 0 32px;
        margin: 0 16px;
        h5 {
          font-size: 18px;
          font-weight: 800;
          margin-bottom: 12px;
        }
        p {
          font-size: 14px;
          font-weight: 400;
        }

      }
    }
  }
}
</style>
