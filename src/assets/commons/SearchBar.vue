<template>
  <div class="search-bar">
      <input v-model="searchText" type="text" placeholder="Inserisci una parola">
      <button @click="$emit('search', searchText)">Cerca</button>
      <button>Reset</button>
  </div>
</template>

<script>
export default {
    name: 'SearchBar',
    data(){
        return{
            searchText: ""
        }
    }

}
</script>

<style lang="scss" scoped>



</style>