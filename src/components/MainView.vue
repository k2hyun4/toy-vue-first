<script setup lang="ts">
import axios from "axios";

const check = async () => {
  const {data} = await axios.get('/check');

  alert(data);
};
</script>

<template>
  <div>
    <p>Hello</p>
    <button @click="check">Check</button>
  </div>
</template>