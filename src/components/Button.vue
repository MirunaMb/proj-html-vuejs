<script>
export default {
  name: 'MyButton',
};
</script>

<template>
  <button class="my-button">
    <slot></slot>
  </button>
</template>

<style scoped>
.my-button {
  width: 10rem;
  height: 4rem;
  background: #303030;
  border: 2px solid #0777df;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #f0ede6;
  font-size: large;
  line-height: 4rem;
  margin: 10px;
  cursor: pointer;
  outline: none;
  transition: background-color 0.3s ease;
}

.my-button:hover {
  background: #0777df;
}
</style>
