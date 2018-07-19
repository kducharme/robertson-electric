<template>
  <nav>
    <p>Robinson Electric</p>
    <ul>
        <li>About</li>
        <li>Services</li>
        <li>Contact</li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: 'Nav',
  data () {
    return {
      msg: "Robinson Electric"
    };
  }
};
</script>

<style lang='scss'>
nav {
  height: 60px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 40px;
  ul {
    list-style: none;
  }
  p {
    color: white;
    font-size: 16px;
    font-weight: 600;
  }
  ul {
      display: flex;
      li {
          margin-right: 16px;
          color: white;
          font-size: 14px;
      }
  }
}
</style>
