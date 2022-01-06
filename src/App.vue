<template>
  <div class="bg-gray-800 text-white h-screen">
    <div class="flex">
      <div class="flex flex-col">
        <NavBar />
      </div>
      <div class="flex flex-col divide-y divide-gray-200 w-screen">
        <SearchBar />
        <Tags />
        <Content />
      </div>
    </div>
  </div>
</template>

<script>

import { library } from '@fortawesome/fontawesome-svg-core';
import { fas } from '@fortawesome/free-solid-svg-icons';
import { fab } from '@fortawesome/free-brands-svg-icons';
import NavBar from './components/NavBar.vue';
import SearchBar from './components/SearchBar.vue';
import Tags from './components/Tags.vue';
import Content from './components/Content.vue';

library.add(fas);
library.add(fab);

export default {
  name: 'App',
  components: {
    NavBar,
    SearchBar,
    Tags,
    Content,
  },
  data() {
    return {
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
