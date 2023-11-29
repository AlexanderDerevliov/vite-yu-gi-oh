<script>
import { store } from '../store';

export default {
    nome: 'Cerca',
    data(){
        return{
            store
        }
    },
}
</script>

<template>
    <div class="cerca">
        <div class="archetipos">
            <select v-model="store.testoRicerca">
                <option  class="p-3" v-for="(elem, index) in store.arrayArchetipi"  :value="elem">{{ elem }}</option>
            </select>
            <button class="btn btn-primary mx-2 p-1" @click="$emit('Alex')" type="submit">Cerca</button>
        </div>

    </div>
</template>

<style scoperd lang="scss">

    
    
    .cerca{
        height: 60px;
        line-height: 60px;
        padding: 0 30px;
     
    }
</style>