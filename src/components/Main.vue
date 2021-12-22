<template>
    <main>
        <SearchBar/>
        <Lista/>
    </main>
</template>

<script>

import Lista from '../assets/commons/Lista.vue';
import SearchBar from '../assets/commons/SearchBar.vue';

export default {
    name: 'Main',
    components: {
        Lista,
        SearchBar
    }
}
</script>

<style lang="scss" scoped>

    main{
        padding: 40px;
        background-color: lightblue;
    }

</style>