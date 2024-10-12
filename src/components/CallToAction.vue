<script setup lang="ts">
import { Icon } from '@iconify/vue';
defineProps<{
  message: string
}>()
</script>

<template>
  <a style="display: flex; align-items: center; color: #07969E; font-size: 20px;">
    {{ message }}
    <Icon icon="material-symbols-light:arrow-right-alt-rounded" style="font-size: 25px;" />
  </a>
</template>
