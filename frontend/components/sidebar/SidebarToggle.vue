<template>
  <div
    class="text-light-distinct-text dark:text-light-distinct-text rounded-md hover:text-light-text dark:hover:text-dark-text"
  >
    <Icon
      v-if="chevronDirection == 'left'"
      name="bi:chevron-bar-left"
      :size="iconSize"
    />
    <Icon
      v-if="chevronDirection == 'right'"
      name="bi:chevron-bar-right"
      :size="iconSize"
    />
  </div>
</template>

<script setup lang="ts">
defineProps<{
  chevronDirection: "left" | "right";
  iconSize: string;
}>();
</script>
