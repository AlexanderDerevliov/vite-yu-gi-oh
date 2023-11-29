<script >

  export default {
    name: 'Card',
    props:['characters']
  }
</script>

<template>
    <div class="card">
        <img :src="characters.card_images[0].image_url" alt="characters">
        <h3 class="nome mt-2">{{ characters.name }}</h3>
        <h4 class="tipo">{{ characters.type }}</h4>
        <h4 class="archetipo mt-1">{{ characters.archetype }}</h4>
    </div>
</template>

<style lang="scss" scoped>
    .card{
        text-align: center;
        width: calc((100% / 5) - 10px);
        margin-top: 20px;
        padding: 20px;
        border-radius: 20px;
        .tipo{
          color:rgb(39, 34, 139);
        }
        .archetipo{
          color: gray;
        }
    }
</style>