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

  </div>
</template>

<script>
import Nav from './Nav.vue';

export default {
  name: 'Home',
  components: {
    Nav
  },
  data() {
    return {
      msg: 'Quality, transparent electrical services in Central MA.',
      sub:
        'At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium voluptatum deleniti atque corrupti quos dolores et quas molestias excepturi.'
    };
  }
};
</script>

<style lang='scss'>
h1, h2, h3, h4, p {
  color: #343849;
}

.home {
  width: 100vw;
  .home__hero {
    background: 
    linear-gradient(
      rgba(52,56,73,0.55), 
      rgba(52,56,73,0.30)
    ),
    url('../img/hero3.jpg');
    background-size: cover;
    min-height: 65vh;
    max-height: 80vh;

    display: flex;
    flex-direction: column;
    justify-content: center;
    height: calc(75vh);
    top: 0;
    padding: 0 100px;
    padding-top:40px;
    // background: rgba(52,56,73,0.50);
    h1 {
      font-family: 'Merriweather';
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
    border-bottom: 1px solid #E2E2E2;
    background-color: #F7F8F9;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 320px;
    p {
      font-size: 14px;
      font-weight: 600;
      color: #6C6C6C;
    }
  }
  .home__about {
    display: flex;
    align-items: center;
    padding: 40px 150px;
    height: 450px;
    .left {
      display: flex;
      justify-content: flex-end;
      width: 50%;
      margin-right: 3%;
      img {
        height: 300px;
        width: auto;
        border-radius: 10px;
        box-shadow: 0 4px 10px 0 rgba(0,0,0,0.15);
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
        margin-bottom: 12px;
      }
      p {
        font-size: 15px;
        line-height: 1.7;
        opacity: .7;
      }
    }
  }
}
</style>
