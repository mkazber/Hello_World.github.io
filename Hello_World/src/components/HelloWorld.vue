<template>
  <div class="greetings">
    <h1 class="green">Cześć Natalia</h1>
    <h3>
      Jesteś piękna
      <a href="https://vitejs.dev/" target="_blank" rel="noopener">Twarz</a> +
      <a href="https://vuejs.org/" target="_blank" rel="noopener">brwi</a>. What's next?
    </h3>
  </div>
</template>

<script setup lang="ts">
defineProps<{
  msg: string
}>()
</script>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
