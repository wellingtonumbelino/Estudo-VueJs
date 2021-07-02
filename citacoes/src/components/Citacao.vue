<template>
  <div class="citacao">
    <slot name="fonte"></slot>
    <slot name="texto"></slot>
    <div class="autor"><slot name="autor"></slot></div>
  </div>
</template>

<script>
export default {
  props: ["texto"],
};
</script>

<style scoped>
.citacao {
  border: 1px solid #ddd;
  background-color: rgba(0, 0, 0, 0.1);
  padding: 25px;
  max-width: 450px;
}

.autor {
  float: right;
}
</style>
