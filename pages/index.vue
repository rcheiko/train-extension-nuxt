<template>
    <div>
        <h1 class="text-2xl font-semibold">Hello</h1>
        <p>How are you</p>
    </div>
</template>

<script setup lang="ts">
definePageMeta({
    title: 'base.meta.home.title',
    description: 'base.meta.home.description'
});

if (chrome.storage) {
    chrome.storage.sync.set({ color: '#3aa757' }, function () {
        console.log('The color is green.');
    });
}
</script>