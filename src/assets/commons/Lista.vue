<template>
  <div class="lista">
      <Oggetto :Oggetti="Oggetti"/>
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
    props: {
        Oggetti: Array
    }
}
</script>

<style lang="scss" scoped>



</style>