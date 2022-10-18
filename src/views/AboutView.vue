<script setup>
import {useCounterStore} from "@/stores/counter";

const counterStore = useCounterStore()
</script>

<template>
  <div class="about">
    <h1>About</h1>
    <button @click="counterStore.increaseCount" class="counter-btn">{{counterStore.count}}</button>
  </div>
</template>

<style>
.counter-btn {
  font-size: 60px;
  margin: 20px;
}
</style>
