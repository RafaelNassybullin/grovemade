<template>
  <div class="wrap" v-for="item in largeCardData" :key="item.id">
    <div class="image">
      <img :src="require('../assets/img/'+item.image)" alt="">
    </div>
    <div class="large-card-text">
      <h2>{{ item.name }}</h2>
      <button>LEARN MORE</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "largeCards",
  data() {
    return {
      largeCardData: [
        {image: "ca3ca2fb31735a13f73a37e2560bd0ee.webp", name: 'Desk Pads', id: 24},
        {image: "bfc516c8c76d7976a8570d5e64b6c530.webp", name: 'Laptop Stands', id: 25}
      ]
    }
  },
  computed: {},
  mounted() {
  }
}
</script>

<style scoped lang="scss">
.wrap {
  width: 45.625vw;
  height: 39.583vw;
  margin: 0.833vw;
  @media(max-width: 433px) {
    width: 100%;
    height: 103.583vw;
  }

  .image {
    width: 100%;
    height: 30.556vw;
    overflow: hidden;
    @media(max-width: 433px) {
      height: 62.556vw;
    }

    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      transition: 300ms ease-in-out;
      transition-property: transform;
      @media(max-width: 433px) {

      }

      &:hover {
        transform: scale(1.06);
      }
    }
  }

  .large-card-text {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    height: 9.653vw;
    @media(max-width: 433px) {
      height: 31.653vw;
    }
  }

  h2 {
    margin-bottom: 2vw;
    font-size: 1.875vw;
    @media(max-width: 433px) {
      font-size: 7.875vw;
      margin-bottom: 3vw;
    }
  }

  button {
    background: transparent;
    outline: none;
    border: none;
    letter-spacing: 0.097vw;
    font-size: 0.903vw;
    text-transform: uppercase;
    font-weight: 500;
    @media(max-width: 433px) {
      font-size: 3.903vw;
    }
  }
}
</style>