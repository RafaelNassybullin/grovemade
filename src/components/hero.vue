<template>
  <main>
    <div class="image">
      <img :src="require('../assets/img/'+images[p])" alt="">
    </div>
    <titles titlee="The Desk Shelf System"
            paragr="Available in Walnut or Maple"
            button="LEARN MORE"
            colour="white"
    ></titles>
  </main>
</template>

<script>
import titles from '@/components/titles'

export default {
  name: "hero",
  data() {
    return {
      gh: true,
      images: [
        "d6892bf250f71554ecc7ec7b6a67093e.jpg",
        "ae1f7d93b3435505b6162394705605c1.jpg"
      ],
      p: 0,
      scrollPosition: Number,
      screen: Number,
      result: Number
    }
  },
  components: {
    titles
  },
  mounted() {
    window.addEventListener('scroll', this.updateScroll)
    window.addEventListener('resize', this.updateScroll)
  },
  destroy() {
    window.removeEventListener('scroll', this.updateScroll)
    window.removeEventListener('resize', this.updateScroll)
  },
  computed: {},
  methods: {
    updateScroll() {
      this.scroll = window.scrollY

      this.screen = window.innerWidth

      this.result = this.scroll / this.screen * 100

      // console.log(this.result.toFixed(3));


      this.screen>433?
          (this.result.toFixed(3) > 35
              ? this.gh = false
              : this.gh = true)
          :(this.result.toFixed(3) > 230
              ? this.gh = false
              : this.gh = true
          )

      this.p = this.gh ? 0 : 1
    }
  }
}
</script>

<style scoped lang="scss">
main {
  width: 100%;
  height: 35.000vw;
  position: relative;
  overflow: hidden;
  @media(max-width: 433px) {
    height: 149vw;
  }

  .image {
    width: 100%;
    height: 35.000vw;
    position: absolute;
    top: 0;
    left: 0;
    z-index: -6;
    @media(max-width: 433px) {
height: 145vw;
    }

    img {
      width: 100%;
      height: 100%;
      top: 0;
      left: 0;
      object-fit: cover;
      position: fixed;
      z-index: -6;
      @media(max-width: 433px) {
        height: 149vw;
      }
    }
  }
}


</style>