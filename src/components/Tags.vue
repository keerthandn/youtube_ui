<template>
<div class="flex space-x-2 py-4">
    <div v-for="item in tags" :key="item" class="border borde-gray-50 px-2 rounded-full bg-gray-600 hover:bg-gray-400">{{item}}</div>
</div>
</template>

<script>
export default {
  name: 'Tags',
  data() {
    return {
      tags: [
        'all',
        'live',
        'coding',
        'vue',
        'typescript',
        'rust',
        'javascript',
        'react',
        'vue.js',
        'programming',
      ],
    };
  },
};
</script>

<style>

</style>
