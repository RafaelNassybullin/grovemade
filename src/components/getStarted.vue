<template>
  <section>
    <titles titlee="Design Inspires"
            paragr="Build your dream workspace, so you can get your best work done."
            button="GET STARTED"
            colour="black"
    ></titles>
    <div class="wrapp">
      <largeCards></largeCards>
    </div>
  </section>
</template>

<script>
import titles from '@/components/titles'
import largeCards from '@/components/largeCards'
export default {
  name: "getStarted",
  components:{
    titles,
    largeCards
  }
}
</script>

<style scoped lang="scss">
  section{
    width: 100%;
    background: white;
    padding: 5.556vw 0;
    .wrapp{
      display:flex;
      align-items:center;
      justify-content:center;
      margin-top: 5.556vw;
    }
  }
</style>