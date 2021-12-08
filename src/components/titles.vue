<template>
  <div class="text" :style="{color:$props.colour}">
    <h1>{{ $props.titlee }}</h1>
    <p :style="{color: $props.paragraphColour}">{{ $props.paragr }}</p>
    <button :style="{color: $props.colour}">{{ $props.button }}</button>
  </div>
</template>

<script>
export default {
  name: "titles",
  props: {
    titlee: '',
    paragr: '',
    button: '',
    colour: '',
    paragraphColour: ''
  }
}
</script>

<style scoped lang="scss">
.text {
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  z-index: 2;
  @media(max-width: 433px) {

  }

  h1 {
    font-size: 2.986vw;
    font-weight: 400;
    margin-bottom: 1.597vw;
    @media(max-width: 433px) {
      font-size: 10.986vw;
      font-weight: 401;
      margin-bottom: 6.597vw;
      text-align: center;
      margin-top: 3vw;
    }
  }

  p {
    font-size: 1.042vw;
    font-weight: 400;
    margin: 0.833vw 0 1.944vw 0;
    text-align: center;
    @media(max-width: 433px) {
      margin: 5.833vw 4vw 14.944vw 4vw;
      font-size: 5.042vw;
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
      font-size: 4.903vw;
    }
  }

}
</style>