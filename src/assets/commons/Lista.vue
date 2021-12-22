<template>
  <div class="lista">
      <Oggetto/>
      <h1>contenuto lista</h1>
  </div>
</template>

<script>

import Oggetto from '../commons/Oggetto.vue';

export default {
    name: 'Lista',
    components: {
        Oggetto
    },
    data(){
        return{
            Oggetti: []
        }
    },
    created(){
        
    }
}
</script>

<style lang="scss" scoped>



</style>