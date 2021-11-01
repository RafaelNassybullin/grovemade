<template>
  <navbar></navbar>
  <hero></hero>
  <getStarted></getStarted>

</template>


<script>
import navbar from "@/components/navbar";
import hero from "@/components/hero";
import getStarted from "@/components/getStarted";
export default {

  components:{
    navbar,
    hero,
    getStarted
  }
}



</script>
<style lang="scss">
  *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  body{
    font-family: Roboto, sans-serif;
  }



</style>
