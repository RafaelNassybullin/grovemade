<template>
  <section class="wrap">
    <div class="text-meaningful">
      <titles titlee="Make Work Meaningful"
              paragr="We're here because we believe that your work deserves the best. A team that loves working together is the magic that makes it all happen."
              colour="black"
              paragraphColour="gray"
      >

      </titles>
    </div>
    <div class="images-container">
      <div class="imagees" v-for="item in imageData">
        <img :src="require('../assets/img/'+item)" alt="">
      </div>
    </div>
  </section>
</template>
<script>
import titles from '@/components/titles'

export default {
  data() {
    return {
      imageData: [
        '1.jpg',
        '2.jpg',
        '3.jpg',
        '4.jpg',
        '5.jpg',
        '6.jpg',
        '7.jpg',
        '8.jpg',
        '9.jpg',
        '10.jpg',
        '11.jpg',
        '12.jpg',
        '13.jpg',
        '14.jpg',
        '15.jpg',
        '16.jpg',
        '17.jpg',
        '18.jpg'
      ]
    }
  },
  components: {
    titles
  }
}
</script>
<style scoped lang="scss">
.wrap {
  background: white;
  display:flex;
  align-items:center;
  justify-content:center;
  flex-direction: column;
  @media(max-width: 433px){

  }
}

.text-meaningful {
  width: 54.792vw;
  @media(max-width: 433px){
    width: 93.792vw;
  }
}

.images-container {
  width: 94.792vw;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-wrap: wrap;
@media(max-width: 433px){
width: 92.792vw;
  }
  .imagees {
    width: 13.889vw;
    height: 18.819vw;
    overflow: hidden;
    margin: 0.8vw;
@media(max-width: 433px){
width: 24.889vw;
height: 35.819vw;
  margin: 2.8vw;
  }
    img {
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
}
</style>