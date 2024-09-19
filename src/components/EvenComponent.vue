<script setup>
const handleClick = () => {
  console.log("clicked");
};

const handleDelete = (id) => {
  console.log("id", id);
};

const handleGetEvent = (event) => {
  console.log("event info", event);
};

const handleSubmit = () => {
  alert("Submit");
};

const handleCloseForm = () => {
  console.log("close form");
};
</script>

<template>
  <button v-on:click="handleClick">click me</button>
  <button v-on:click="handleDelete(1)">Delete</button>
  <button @click="handleGetEvent">event info</button>

  <form @submit.prevent="handleSubmit">
    <!-- ngan chan hanh dong load lai trang -->
    <button type="submit">submit</button>
  </form>

  <button @keydown.esc="handleCloseForm">dong form</button>
</template>

<style>

</style>
