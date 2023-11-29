<script>
import { store } from '../store';

export default {
    nome: 'Cerca',
    data() {
        return {
            store
        }
    },
}
</script>

<template>
    <div class="cerca">
        <div class="archetipos">
            <select v-model="store.testoRicerca">
                <option class=" option_cerca p-3" v-for="(elem, index) in store.arrayArchetipi" :value="elem">{{ elem }}
                </option>
            </select>
           
        </div>

    </div>
</template>

<style lang="scss" scoped>
.cerca {
    height: 60px;
    line-height: 60px;
    padding: 0 30px;
  
}
select {
    min-height: 32px;
    border-radius: 10px;
}
</style>
