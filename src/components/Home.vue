<template>
  <div class='home'>
    <Nav />
    <div class='home__hero'>
      <h1>{{ msg }}</h1>
      <p>{{ sub }}</p>
      <button>Request a quote</button>
    </div>

    <div class="home__announce">
      <p>ryanrobinson@gmail.com</p>
      <p>(508) 555-5555</p>
      <p>facebook.com/robinsonelectric</p>
    </div>

    <div class="home__about">
      <div class="left">
        <img src="../img/hero2.jpg" alt="">
      </div>
      <div class="right">
        <h2>About Robinson Electric</h2>
        <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione voluptatem sequi nesciunt.</p>
      </div>
    </div>

    <div class="home__services">
      <div class="top">
        <h2>Electrical Services</h2>
        <p>At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium voluptatum deleniti atque corrupti quos dolores et quas molestias excepturi sint occaecati cupiditate non provident.</p>
      </div>
      <div class="bottom">
        <div class="left card">
          <img src="../img/residential.svg" alt="">
          <h4>Residential</h4>
          <p>At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium voluptatum deleniti atque.</p>
        </div>
        <div class="right card">
          <img src="../img/commercial.svg" alt="">
          <h4>Commercial</h4>
          <p>At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium voluptatum deleniti atque.</p>
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
      msg: "Quality, transparent electrical services in Central MA.",
      sub:
        "At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium voluptatum deleniti atque corrupti quos dolores et quas molestias excepturi."
    };
  }
};
</script>

<style lang='scss'>
h1,
h2,
h3,
h4,
p {
  color: #343849;
}

.home {
  width: 100vw;
  .home__hero {
    background: linear-gradient(rgba(52, 56, 73, 0.55), rgba(52, 56, 73, 0.3)),
      url("../img/hero3.jpg");
    background-size: cover;
    min-height: 65vh;
    max-height: 80vh;

    display: flex;
    flex-direction: column;
    justify-content: center;
    height: calc(75vh);
    top: 0;
    padding: 0 100px;
    padding-top: 40px;
    // background: rgba(52,56,73,0.50);
    h1 {
      font-family: "Merriweather";
      width: 48vw;
      font-size: 40px;
      color: white;
      line-height: 1.4;
      margin-bottom: 16px;
    }
    p {
      line-height: 1.7;
      width: 48vw;
      color: white;
      font-size: 18px;
      font-weight: 400;
      margin-bottom: 48px;
    }
    button {
      height: 52px;
      width: 160px;
      font-size: 16px;
      font-weight: 600;
      background-color: #ff3a20;
      color: white;
      font-weight: 600;
      border: none;
      border-radius: 5px;
    }
    button:hover,
    button:active {
      background-color: rgb(219, 50, 28);
      cursor: pointer;
    }
  }
  .home__announce {
    height: 60px;
    border-bottom: 1px solid #e2e2e2;
    background-color: #f7f8f9;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 320px;
    p {
      font-size: 14px;
      font-weight: 600;
      // color: #6C6C6C;
    }
  }
  .home__about {
    display: flex;
    align-items: center;
    padding: 100px 150px;
    // height: 500px;
    border-bottom: 1px solid #e2e2e2;
    .left {
      display: flex;
      justify-content: flex-end;
      width: 50%;
      margin-right: 3%;
      img {
        height: 300px;
        width: auto;
        border-radius: 10px;
        box-shadow: 0 4px 10px 0 rgba(0, 0, 0, 0.15);
      }
    }
    .right {
      display: flex;
      justify-content: flex-start;
      width: 50%;
      margin-left: 3%;
      flex-direction: column;
      h2 {
        font-size: 28px;
        margin-bottom: 18px;
      }
      p {
        font-size: 15px;
        line-height: 1.7;
        opacity: 0.7;
      }
    }
  }
  .home__services {
    display: flex;
    flex-direction: column;
    padding: 60px 0;
    border-bottom: 1px solid #e2e2e2;
    background-color: #F7F8F9;
    .top {
      padding: 0px 150px;
      margin-bottom: 32px;
      text-align: center;
      h2 {
        margin-bottom: 18px;
        font-size: 28px;
      }
      p {
        opacity: 0.7;
        font-size: 15px;
        line-height: 1.7;
        width: 70%;
        margin: auto;
      }
    }
    .bottom {
      display: flex;
      justify-content: center;
      padding: 0px 150px;
      .card {
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        text-align: center;
        padding: 32px;
        border: 1px solid #e2e2e2;
        border-radius: 5px;
        width: 25%;
        margin: 32px;
        min-height: 280px;
        min-width: 280px;
        background-color: white;
        img {
          height: 50px;
          width: auto;
          margin-bottom: 16px;
        }
        h4 {
          font-size: 20px;
          font-weight: 600;
          margin-bottom: 8px;
        }
        p {
          font-size: 14px;
          opacity: .7;
          line-height: 1.3;
        }
      }
    }
  }
}
</style>
