<template>
  <main>
    <div class="image">
      <img src="../assets/img/d6892bf250f71554ecc7ec7b6a67093e.jpg" alt="">
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
  components:{
    titles
  }
}
</script>

<style scoped lang="scss">
main {
  width: 100%;
  height: 35.000vw;
  position: relative;
  overflow: hidden;

  .image {
    width: 100%;
    height: 35.000vw;
    position: absolute;
    top: 0;
    left: 0;
    z-index: -6;

    img {
      width: 100%;
      height: 100%;
      top: -3vw;
      object-fit: cover;
      position: fixed;
      z-index: -6;
    }
  }
}


</style>