<script>
import axios from "axios";

export default {
  created(){
    axios.get ("https://db.ygoprodeck.com/api/v7/cardinfo.php?num=20&offset=0") 
    .then ((resp) => {
      console.log(resp)
    });
  }
   
  }


</script>

<template>
<h1>Hello</h1>
</template>

<style lang="scss" >
@use "./style/general.scss"

</style>
