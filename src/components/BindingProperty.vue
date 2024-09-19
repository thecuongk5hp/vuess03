<template>
  <img v-bind:src="url" alt="" />
  <!-- <img :src="url" alt="" /> -->

  <button v-bind:disabled="isDisabled">Click me</button>

  <input type="text" v-bind:disabled="isEnter" />

  <div v-bind="divAttributes">container</div>

  <!-- binding 2 thuoc tinh id : "paragraph", area="paragraph" -->
  <p v-bind="paragraphAttributes">noi dung</p>

  <!-- v-bind cho class va style -->
  <div v-bind:class="{textRed: isTextRed}">Hello world</div>

</template>

<script setup>
const url =
  "https://th.bing.com/th/id/R.5b7f7813baf8192b1b663769e14b6a80?rik=gERF1pQoSregqA&pid=ImgRaw&r=0";
const isDisabled = false;

const isEnter = false;

const divAttributes = {
  id: "container-id",
  class: "container-class",
};

const paragraphAttributes = {
  id: "paragraph",
  area: "paragraph",
};
const isTextRed = true;
</script>

<style>
.textRed {
  color:red
}
</style>
