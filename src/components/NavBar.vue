<template>
    <div v-for="item in navbar" :key="item.name">
        <div class="flex flex-col place-items-center hover:bg-gray-600 p-4">
        <div>
            <fa :icon="item.icon" class="text-3xl" />
        </div>
        <div class="text-sm">
            {{ item.name }}
        </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'NavBar',
  data() {
    return {
      navbar: [
        {
          name: '',
          icon: 'bars',
        },
        {
          name: 'home',
          icon: 'home',
        },
        {
          name: 'explore',
          icon: 'compass',
        },
        {
          name: 'subscriptions',
          icon: 'photo-video',
        },
        {
          name: 'library',
          icon: 'window-restore',
        },
        {
          name: 'history',
          icon: 'history',
        },
      ],
    };
  },
};
</script>
