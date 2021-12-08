<template>
  <navbar/>
  <hero/>
  <getStarted/>
  <featureproducts/>
  <homeoffice/>
  <hardWay/>
  <meaningfull/>
  <jointous/>
  <foooter/>
</template>


<script>
import navbar from "@/components/navbar";
import hero from "@/components/hero";
import getStarted from "@/components/getStarted";
import hardWay from "@/components/hardWay";
import meaningfull from "@/components/Meaningfull";
import jointous from "@/components/JoinToUs";
import featureproducts from "@/components/FeatureProducts";
import homeoffice from "@/components/HomeOffice";
import foooter from "@/components/Foooter";

export default {

  components:{
    navbar,
    hero,
    getStarted,
    hardWay,
    meaningfull,
    jointous,
    featureproducts,
    homeoffice,
    foooter
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
