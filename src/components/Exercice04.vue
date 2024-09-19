<template>
  <div v-bind:class="{active: isActive}">block</div>
</template>

<script setup>
</script>
const isActive = true;
<style>
.active {
    color : blue;
}
</style>