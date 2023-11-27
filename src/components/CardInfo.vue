
<script>
import { store } from '../store';
import AppCards from './AppCards.vue';

export default {
    data() {
        return {
            store
        };
    },
    components: { AppCards }
}
</script>

<template>
<div class="container">
    
    <div class="row">
        <div class="col" v-for="data in store.data" :key="data.id">
            
        <AppCards :data="data" /> 

        </div>
    </div>
</div>
</template>


<style lang="scss" scoped>

</style>