<template>
    <div class="text" :style="{color:$props.colour}">
      <h1>{{ $props.titlee }}</h1>
      <p>{{ $props.paragr }}</p>
      <button :style="{color:$props.colour}">{{ $props.button }}</button>
    </div>
</template>

<script>
export default {
  name: "titles",
  props:{
    titlee:'',
    paragr:'',
    button:'',
    colour:''
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

h1 {
  font-size: 2.986vw;
  font-weight: 400;
}

p {
  font-size: 1.042vw;
  font-weight: 400;
  margin: 0.833vw 0 1.944vw 0;
}

button {
  background: transparent;
  outline: none;
  border: none;
  letter-spacing: 0.097vw;
  font-size: 0.903vw;
  text-transform: uppercase;
  font-weight: 500;
}

}
</style>