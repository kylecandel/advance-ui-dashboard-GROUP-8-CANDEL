<script setup>
defineProps({
  title: String,
  label: String
})
</script>

<template>
  <div class="card">
    <button :aria-label="label">{{ title }}</button>
  </div>
</template>

<style scoped>
.card {
  background: #1e293b;
  padding: 20px;
  border-radius: 8px;
  color: white;
  text-align: center;
  font-weight: bold;
}

.card button {
  width: 100%;
  padding: 15px;
  border: none;
  background: transparent;
  color: white;
  font-size: 16px;
  cursor: pointer;
}

button:focus {
  outline: 3px solid #38bdf8;
}
</style>