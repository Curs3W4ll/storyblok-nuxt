<script setup lang="ts">
const story = await useStoryblok('vue/test', { version: 'draft' });
</script>

<template>
  <StoryblokComponent v-if="story" :blok="story.content" />
</template>
