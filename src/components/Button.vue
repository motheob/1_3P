<template>
  <button class="button" @click="handleClick">
    <slot></slot>
  </button>
</template>

<script>
export default {
  methods: {
    handleClick() {
      this.$emit('click');
    },
  },
};
</script>

<style scoped>
.button {
  background-color: #6e7e8d;
  color: #fafaf7;
  padding: 10px 20px;
  border: none;
  cursor: pointer;
  border-radius: 3px;
}
</style>