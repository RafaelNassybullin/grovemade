<template>
  <div class="hard-wrapper">
    <div class="text">
      <titles titlee="Made The Hard Way"
            paragr="Our signature craftsmanship has been honed over a decade of manufacturing innovation here in Portland, Oregon. We combine the skills of our small in-house team with the collective strength of collaborators throughout the US to deliver quality products worth investing in."
            colour="black"
              lineHeight="1.667vw"
              paragraphColour="gray"
    ></titles>
    </div>
    <div class="hard-image">
      <img src="../assets/img/d8aa033ae2f00d15207e1e61d3181812.jpg" alt="">
    </div>
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
.hard-wrapper{
  background: white;
  display:flex;
  align-items:center;
  justify-content:center;
  flex-direction: column;
  padding-bottom: 2.778vw;
  @media(max-width: 433px){

  }
}
.text{
  width: 53.958vw;
  margin-top: 2vw;
  @media(max-width: 433px){
    width: 95.958vw;
  }
}
.hard-image{
  width: 73.056vw;
  height: 41.111vw;
  background: pink;
  overflow: hidden;
  @media(max-width: 433px){
    width: 96.056vw;
height: 56.111vw;
  }
  img{
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: 300ms ease-in-out;
      transition-property: transform;
    @media(max-width: 433px){

  }
      &:hover{
        transform: scale(1.06);
      }
  }
 }
</style>