
<script>
import { store } from '../store';

export default {
    data(){
        return {
            store

        }
    }
}
</script>

<template>
<div class="container">
    <div class="row">
        <div class="col" v-for="infoCards in store.infoCards">
            {{ infoCards.name }}

        </div>
    </div>
</div>
</template>


<style lang="scss" scoped>

</style>