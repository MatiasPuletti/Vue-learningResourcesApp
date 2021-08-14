<template>
  <button :class="mode">
    <slot></slot>
  </button>
</template>

<script>
export default {
  props: ['mode']
};
</script>

<style scoped>
button {
  padding: 0.75rem 1.5rem;
  font-family: inherit;
  background-color: #2e8bc0;
  border: 1px solid #2e8bc0;
  color: white;
  cursor: pointer;
  border-radius: 5px;
}

button:hover,
button:active {
  background-color: #0c2d48;
  border-color: #0c2d48;
}

.flat {
  background-color: transparent;
  color: #3a0061;
  border: none;
}

.flat:hover,
.flat:active {
  background-color: #0c2d48;
  color: white;
}
</style>
