<template>
  <div class="feature-container">
    <titles
        titlee="Featured Products"
        paragr="See What’s Trending Right Now"
        paragraphColour="#A0A0A0"
    />
    <div class="pagi">
      <span class="bull"></span>
      <span class="bull"></span>
      <span class="bull"></span>
    </div>
    <div class="container-slider">
      <swiper :pagination="screenSize>433?{ clickable: true, el:'.pagi', bulletClass:'bull'}:false"
              class="mySwiper"
              :slidesPerView="screenSize>433?4:1"
              :slides-per-group="screenSize>433?4:1"
              :loop="true"
      >
        <swiper-slide v-for="item in colors" class="swiper-slide">
          <div class="conti">
            <div class="swip-image">
              <img :src="require('../assets/img/'+item.image)" alt="">
            </div>
            <div class="swip-text">
              <p class="name">{{ item.name }}</p>
              <p>{{ item.price }} $</p>
            </div>
          </div>
        </swiper-slide>
      </swiper>
    </div>
  </div>
</template>

<script>
import {Swiper, SwiperSlide} from 'swiper/swiper-vue.esm'
import SwiperCore, {Navigation, Pagination} from "swiper";
import "swiper/swiper-bundle.min.css";

SwiperCore.use([Pagination, Navigation]);
import titles from '@/components/titles'

export default {
  components: {
    titles,
    Swiper,
    SwiperSlide
  },
  data() {
    return {
      colors: [
        {image: 'slide1.png', name: 'Walnut MagSafe Stand', price: 120},
        {image: 'slide2.png', name: 'Walnut Laptop Riser', price: 150},
        {image: 'slide3.png', name: 'Walnut iPad Stand', price: 80},
        {image: 'slide4.png', name: 'Walnut Monitor Stand', price: 100},
        {image: 'slide1.png', name: 'Walnut MagSafe Stand', price: 120},
        {image: 'slide2.png', name: 'Walnut Laptop Riser', price: 150},
        {image: 'slide3.png', name: 'Walnut iPad Stand', price: 80},
        {image: 'slide4.png', name: 'Walnut Monitor Stand', price: 100},
        {image: 'slide1.png', name: 'Walnut MagSafe Stand', price: 120},
        {image: 'slide2.png', name: 'Walnut Laptop Riser', price: 150},
        {image: 'slide3.png', name: 'Walnut iPad Stand', price: 80},
        {image: 'slide4.png', name: 'Walnut Monitor Stand', price: 100},
      ],
      screenSize:window.innerWidth
    }
  },
  mounted() {
    window.addEventListener('resize', this.resized)
  },
  destroy() {

    window.removeEventListener('resize', this.resized)
  },

  methods:{
    resized(){
      this.screen = window.innerWidth
      this.screenSize = this.screen
      // console.log(this.screenSize);
    }
  }
}
</script>

<style lang="scss">
.feature-container {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  background: white;
  @media(max-width: 433px) {

  }
}

.conti {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  @media(max-width: 433px) {

  }

  .swip-text {
    align-self: flex-start;
    font-size: 0.868vw;
    margin-left: 1.3vw;
    color: #A0A0A0;
    @media(max-width: 433px) {
      font-size: 6.868vw;
      margin-left: 3.3vw;
    }

    .name {
      margin-bottom: 0.556vw;
      //text-align: center;
      @media(max-width: 433px) {
        margin-bottom: 2.556vw;
      }
    }
  }
}

.container-slider {
  width: 93.056vw;
  height: 34.236vw;
  margin-bottom: 6.944vw;
  @media(max-width: 433px) {
    height: 112.236vw;
  }
}

.swiper-slide {
  height: 34.236vw;
  cursor: pointer;
  @media(max-width: 433px) {
    height: 110.236vw;
  }

  .swip-image {
    width: 20.528vw;
    height: 28.139vw;
    margin: 0.868vw;
    overflow: hidden;
    @media(max-width: 433px) {
      width: 92.528vw;
      height: 84.139vw;
      margin: 3.868vw;
    }

    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      transition: 300ms ease-in-out;
      transition-property: transform;

      &:hover {
        transform: scale(1.06);
      }
    }
  }
}

.pagi {
  display: flex;
  align-items: center;
  justify-content: center;
  @media(max-width: 433px) {

  }
}

.bull {
  background: black;
  width: 0.486vw;
  height: 0.486vw;
  margin: 0.556vw;
  @media(max-width: 433px) {
    width: 3.486vw;
    height: 3.486vw;
    margin: 2.556vw;
  }
}

.swiper-pagination-bullet-active {
  background: gray;
  @media(max-width: 433px) {

  }
}
</style>