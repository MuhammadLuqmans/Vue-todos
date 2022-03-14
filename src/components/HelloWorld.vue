<script setup lang="ts">
import { ref, onMounted, computed } from 'vue'

// reactive state
const count = ref(0)

// const condition = computed( ()=>{
//   return 
// })
// functions that mutate state and trigger updates
function increment() {
  count.value++
  // condition()
}
const decrement = () => {
  count.value--
  // condition()
}

// lifecycle hooks
onMounted(() => {
  console.log(`The initial count is ${count.value}.`)
})
</script>

<template>
  <h2>Count is: {{ count }}</h2>
  
  <div>{{count >= 10 ? ' Luqman 10' :'luqman less 10'}}</div>
  <button @click="increment">Increase Amount</button>
  <button @click="decrement">Decrease Amount</button>
</template>