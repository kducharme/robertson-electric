<template>
  <nav>
    <p>Robinson Electric</p>
    <ul>
        <li>Services</li>
        <li>About</li>
        <li>Reviews</li>
        <!-- <button>Contact me</button> -->
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
  padding: 0 100px;
  background-color: white;
  z-index: 999;
  position: fixed;;
  width: 100vw;
  ul {
    list-style: none;
  }
  p {
    color: #343849;
    font-size: 18px;
    font-weight: 600;
  }
  ul {
      display: flex;
      align-items: center;
      li {
          margin-right: 24px;
          color: #343849;
          font-size: 14px;
      }
      button {
          height: 40px;
          width: 110px;
          font-size: 14px;
          font-weight: 600;
          background-color: #FF3A20;
          color: white;
          font-weight: 600;
          border: none;
          border-radius: 5px;
      }
      button:hover, button:active {
          background-color: rgb(219, 50, 28);
          cursor: pointer;
      }
  }
}
</style>
