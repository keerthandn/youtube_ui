<template>
<div class="flex text-3xl py-4 pr-4 justify-between">
    <div class="flex space-x-2 place-items-center">
        <div>
            <fa :icon="['fab', 'youtube']" class="text-red-800" />
        </div>
        <div class="font-bold">YouTube</div>
    </div>
    <div class="flex space-x-8 place-items-center">
        <div class="flex bg-black border-solid border border-gray-200">
            <input
                class="bg-black w-96 px-2"
                type="text"
                placeholder="Search"
            />
            <div class="bg-gray-800 px-4 py-1 border-solid border border-gray-200">
                <fa icon="search" />
            </div>
        </div>
        <div>
            <fa icon="microphone" />
        </div>
    </div>
    <div class="flex space-x-8 place-items-center">
        <fa icon="th" />
        <fa icon="ellipsis-v" />
        <div class="flex place-items-center space-x-2 text-blue-500 border-solid border border-blue-500 p-2">
            <div><fa icon="user-circle" /></div>
            <div class="text-xl">SIGN IN</div>
        </div>
    </div>
</div>
</template>

<script>
export default {
  name: 'SearchBar',
};
</script>

<style>

</style>
