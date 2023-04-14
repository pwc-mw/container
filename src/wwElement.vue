<template>
  <div class="container">
    <slot class="my-element"> </slot>
  </div>
</template>

<script>
export default {
  props: {
    content: { type: Object, required: true },
  },
  computed: {
    textStyle() {
      return {
        color: this.content.textColor,
      };
    },
  },
};
</script>

<style lang="scss" scoped>
.container {
  width: 100%;
  position: relative;
  height: inherit;
  color: inherit;
  background-color: inherit;
}
</style>
