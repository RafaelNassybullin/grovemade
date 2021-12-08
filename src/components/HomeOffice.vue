<template>

  <div class="conatiner-home-office">
    <titles
      titlee="Home Office Inspiration"
      paragr="Working from home can be a challenge—see some creative solutions to get it just right."
      button="LEARN MORE"
      colour="white"
    />
  </div>

</template>


<script>
import titles from '@/components/titles'


export default {
  components:{
    titles
  }
}
</script>

<style scoped lang="scss">
.conatiner-home-office{
  padding: 12.569vw 0;
  @media(max-width: 433px){
    padding: 32.569vw 0;
  }
}

</style>