<template>
  <div class="icon-wrapper">
    <span class="material-icons icon" :class="size">{{ name }}</span>
  <div class="icon-wrapper" v-html="svg"></div>
  </div>
</template>

<script>
export default {
  props: {
    name: String,
    size: {
      type: String,
      default: 'medium',
    },
  },
}
</script>

<style scoped>
.icon-wrapper {
  display: inline-flex;
  align-items: center;
  color: rgba(0, 0, 0, 0.4);
}

.icon {
  margin-right: 6px;
}
</style>
