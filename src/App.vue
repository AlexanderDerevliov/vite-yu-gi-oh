<script>
import axios from "axios";
import AppHeader from "./components/AppHeader.vue";
import { store } from "./store.js";
import CharactersList from "./components/CharactersList.vue";

export default {
  data() {
    return {
      store
    };
  },
  created() {
    axios.get("https://db.ygoprodeck.com/api/v7/cardinfo.php?num=20&offset=0")
      .then((resp) => {
        this.store.data = resp.data.results;
      });
  },
  components: { AppHeader, CharactersList }
};


</script>

<template>
  <!-- header -->
  <AppHeader />
  <!-- characters list of cards -->
  <CharactersList />
</template>

<style lang="scss" >
@use "./style/general.scss"
</style>
