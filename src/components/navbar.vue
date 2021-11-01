<template>
  <nav>
    <ul>
      <li>shop</li>
      <li>explore</li>
    </ul>

    <div class="logo">
      <img src="../assets/logo.svg" alt="">
    </div>
    <button>my cart</button>
  </nav>
</template>

<script>
export default {
  name: "navbar",
}
</script>

<style scoped lang="scss">
  nav{
    display:flex;
    align-items:center;
    justify-content:space-between;
    background: #ffffff;
    padding: 0 5.556vw;
    height: 5.208vw;
    position: fixed;
    width: 100%;
    z-index: 6;
    ul{
      display: flex;
      list-style: none;
      font-size: 0.903vw;
      text-transform: uppercase;
      letter-spacing: 0.097vw;
      li{
        margin-right: 1.667vw;
        font-weight: 500;
      }
    }
  }
  button{
    background: transparent;
    outline: none;
    border: none;
    letter-spacing: 0.097vw;
    font-size: 0.903vw;
    text-transform: uppercase;
    font-weight: 500;
  }
  .logo{
    width: 13.889vw;
    height: 1.181vw;
    img{
      width: 100%;
      height: 100%;
      object-fit: contain;
    }
  }
</style>