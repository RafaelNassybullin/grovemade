<template>
  <div class="join-wrapper">
    <titles
        titlee="We Hope You'll Join Us"
        paragr="READ MORE ABOUT OUR STORY"
    />
    <div class="design">
      <div class="logotype">
        <svg height="34px" fill="#fff" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 39.51 33.5">
          <path
              d="M23.12,18.61a4.75,4.75,0,0,1,.66-1.49c.85-1.38,1.79-2.72,2.7-4.06,1-1.53,2.11-3,3.11-4.58a24.22,24.22,0,0,0,2.8-6.12C32.72,1.3,33.17-1,34.61.49c1.71,1.75,2.39,4.84,3,7.12a45.85,45.85,0,0,1,1.77,9.27,61.22,61.22,0,0,1-.35,10.22,7.62,7.62,0,0,1-1.14,3.84,6,6,0,0,1-4,2.28c-3.64.55-5.53-1.82-7.13-4.69-1-1.85-2.08-3.73-2.94-5.66A7,7,0,0,1,23.12,18.61Z"/>
          <path
              d="M17,21c2.49.83,3.47,4.35,4.42,6.47.53,1.2,1.09,2.4,1.53,3.64.16.44.49,1.16.3,1.64-.28.73-1.41.72-2,.75-2.58.11-5.19-.11-7.76-.22a26.91,26.91,0,0,1-6.59-.57,5.38,5.38,0,0,1-3-2.64C3,28.66,2.27,27.22,1.51,25.79A11.8,11.8,0,0,1,0,22.53C-.19,21.32.65,21.05,1.67,21c2.43-.08,4.86-.07,7.29-.16.95,0,1.9,0,2.85,0C13.44,20.81,15.46,20.46,17,21Z"/>
        </svg>
      </div>
      <titles
          titlee="Design Inspires"
          paragr="Build your dream workspace, so you can get your best work done."
          colour="white"
      />
    </div>
  </div>
</template>

<script>
import titles from '@/components/titles'

export default {
  components: {
    titles
  }
}
</script>

<style scoped lang="scss">
.join-wrapper {
  background: white;
  padding: 6.667vw 3.472vw 7.708vw 3.472vw;
  @media(max-width: 433px) {
    padding: 6.667vw 3.472vw 27.708vw 3.472vw;
  }
}

.design {
  width: 100%;
  background: #9AA8B1;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  padding: 8.333vw 0;
  margin-top: 8.333vw;
  @media(max-width: 433px) {
    padding: 25.333vw 0;
  }
}

.logotype {
  margin-bottom: 2.431vw;
  @media(max-width: 433px) {

  }
}
</style>