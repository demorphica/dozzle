<template>
  <div class="columns is-marginless has-text-weight-bold is-family-monospace">
    <span class="column is-ellipsis">
      {{ container.name }}
      <span class="tag is-dark">{{ container.image.replace(/@sha.*/, "") }}</span>
    </span>
  </div>
</template>

<script lang="ts" setup>
defineProps({
  container: Object,
});
</script>

<style lang="scss" scoped></style>
