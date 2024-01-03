<template>
    <div class="hello">
        <h1>{{ msg }}</h1>
        <button @click="getCurrentDate()">GET DATE</button>
        <h4 v-for="num in numbers" :key="num">{{ num }}</h4>
        <button @click="sortNumbers(numbers)">SORT</button>
    </div>
</template>
  
<script setup>
import demo from "@/composables/demo"
import { ref } from "vue"
const msg = ref('');
const numbers = ref([4, 3, 9, 7, 1])

function getCurrentDate() {
    msg.value = demo.getDate();
}

function sortNumbers(nums) {
    numbers.value = demo.sortNumbers(nums);
}
</script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
    margin: 40px 0 0;
}

ul {
    list-style-type: none;
    padding: 0;
}

li {
    display: inline-block;
    margin: 0 10px;
}

a {
    color: #42b983;
}
</style>
  