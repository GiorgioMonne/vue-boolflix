<template>
  <div class="search-bar">
      <input v-model="search" type="text" placeholder="Inserisci una parola">
      <button @klick.prevent="">Cerca</button>
      <button @klick.prevent="">Reset</button>
  </div>
</template>

<script>
export default {
    name: 'SearchBar',
    data(){
        return{
            search: ""
        }
    }

}
</script>

<style lang="scss" scoped>



</style>