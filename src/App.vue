<template>
  <div>
    <div v-for="" class="card">
      <h3>{{ item.name }}</h3>
      <h5>{{ item.price }}</h5>
      <div>
        <button>Купить</button>
        <div>
          <button>-</button>
          <span>Количество</span>
          <button>+</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const color = ref('')
const arr = ref([
  {
    title: 'Зеленый',
    value: 'teal'
  },
  {
    title: 'Красный',
    value: 'red'
  },
  {
    title: 'Синий',
    value: 'blue'
  }
])
</script>

<style scoped>
.first {
  color: red;
}
.second {
  color: teal;
}
</style>
