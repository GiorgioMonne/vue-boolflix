<template>
    <main>
        <SearchBar @search="searching"/>
        <Lista :Oggetti="Oggetti"/>
    </main>
</template>

<script>

import axios from 'axios';
import Lista from '../assets/commons/Lista.vue';
import SearchBar from '../assets/commons/SearchBar.vue';

export default {
    name: 'Main',
    components: {
        Lista,
        SearchBar
    },
    data(){
        return{
            Oggetti: []
        }
    },
    methods: {
        searching(payload){
            axios.get("https://api.themoviedb.org/3/search/movie" , {
                params: {
                    api_key: '087445be9bd2c932d8cc9aa28e2e85be',
                    language: 'it-IT',
                    query: payload
                }
            })
            .then((response) => {
               this.Oggetti = response.data.results;
            })
            .catch((error) => {
                console.log(error)
            });
        }
    }
}
</script>

<style lang="scss" scoped>

    main{
        padding: 40px;
        background-color: lightblue;
    }

</style>