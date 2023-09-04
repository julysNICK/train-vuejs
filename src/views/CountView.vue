<script setup lang="ts">
  import { ref } from 'vue'

  const count = ref(0)

  const increment = () => {
    count.value++
  }

  const decrement = () => {
    count.value--

    if (count.value < 0) {
      count.value = 0
    }
  }
</script>

<template>
  <div class="wrapper">
    <button @click="increment" class="btnPlus">+</button>
    <p>{{ count }}</p>
    <button @click="decrement" class="btnMinus">-</button>
  </div>
</template>

<style scoped>
  
  .wrapper{
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-around;
    width: 100%;
    background-color: #000;
  }

  .btnPlus{
    width: 100px;
    height: 100px;
    border-radius: 50%;
    background-color: #fff;
    border: none;
    outline: none;
    font-size: 2rem;
    font-weight: 700;
    cursor: pointer;
  }

  .btnMinus{
    width: 100px;
    height: 100px;
    border-radius: 50%;
    background-color: #fff;
    border: none;
    outline: none;
    font-size: 2rem;
    font-weight: 700;
    cursor: pointer;
  }

</style>