<template>
  <div class="hero">
    <Nav />
    <div class="hero__cta">
      <h1>{{ msg }}</h1>
    </div>
  </div>
</template>

<script>
import Nav from './Nav.vue'

export default {
  name: 'Home',
  components: {
    Nav
  },
  data () {
    return {
      msg: 'High quality electrical a vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium voluptatum.'
    }
  }
}
</script>

<style lang='scss'>
  .hero {
    background-image: url('../img/hero3.jpg');
    background-size: 100vw;
    width: 100vw;
    height: 80vh;
    .hero__cta {
      display: flex;
      justify-content: center;
      align-items: center;
      height: calc(80vh);
      top: 0;
      margin-top: -60px;
      background: rgba(0,0,0,.3);
      padding: 0 60px;
      text-align: center;
    h1 {
      color: white;
    }
    }
    
  }

</style>
