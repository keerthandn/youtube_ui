<template>
    <div class="flex p-4">
        <div v-for="item in videos" :key="item.title">
            <div class="w-80 p-2">
                <img :src="item.thumbnail" alt="" class="rounded" />
                <div class="flex space-x-2 pt-2">
                    <div class="w-12">
                        <img :src="item.profile_pic" alt="" class="rounded-full" />
                    </div>
                    <div class="flex flex-col">
                        <div class="font-bold">{{ item.title }}</div>
                        <div>{{ item.creator }}</div>
                        <div>{{ item.views }} views . {{ item.upload }}</div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'Content',
  data() {
    return {
      videos: [
        {
          thumbnail: '/images/01.png',
          video_length: '10:05',
          profile_pic: '/images/profile_pic.png',
          title: 'Coding a Tinder for Memes with the Giphy API and Vue.js',
          creator: '@keerthan',
          views: '2.5k',
          upload: '1 day ago',
        },
        {
          thumbnail: '/images/02.png',
          video_length: '10:05',
          profile_pic: '/images/profile_pic.png',
          title: 'Rest API',
          creator: '@keerthan',
          views: '2.5k',
          upload: '1 day ago',
        },
        {
          thumbnail: '/images/03.png',
          video_length: '10:05',
          profile_pic: '/images/profile_pic.png',
          title: 'Spider man no way home',
          creator: '@keerthan',
          views: '2.5k',
          upload: '1 day ago',
        },
      ],
    };
  },
};
</script>

<style>

</style>
