<script >
 import Card from './Card.vue'
 import {store} from '../store'
  export default {
    name: 'AppCharacters',
    components:{
        Card
    },
    data(){
        return{
            store
        }
    }
  }
</script>

<template>
    <div>
        <div class="container">
            <Card v-for="(elem, index) in store.arrayCarte"
            :characters=elem
            />
        </div>
    </div>
</template>

<style lang="scss" scoped>
        
        .container{
            width: 80%;
            margin: 0 auto;
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
        }
    
</style>