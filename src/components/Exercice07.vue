<template>
  <form @submit.prevent="handleSubmit">
    <input type="text">
    <button type="submit">submit</button>

  </form>
</template>

<script setup>
const handleSubmit = () => { 
    alert("Form submission prevented!"); 
};
</script>
<style></style>
