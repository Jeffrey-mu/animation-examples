<script setup lang="ts">
import gsap from 'gsap'

onMounted(() => {
  gsap.to('.box', {
    x: 100,
    y: 100,
  })
})
</script>

<template>
  <div id="container">
    <div class="box">
      <img class="green" src="https://greensock.com/wp-content/uploads/custom/draggable/img/knob.png" alt="">
    </div>
  </div>
</template>

<style>
.box {
    display: block;
    width: 300px;
    height: 300px;
    border: 1px solid red;
    border-radius: 50%;
    text-align: center;
    background-image: url(https://greensock.com/wp-content/uploads/custom/draggable/img/knob_bg.jpg);
    background-size: cover;
  }
  img{
    width: 100%;
  }
</style>
