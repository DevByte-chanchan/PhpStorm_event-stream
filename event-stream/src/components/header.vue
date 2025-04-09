<script setup>
</script>


<template>

  <div class="header">
    <img height="48" src="@/assets/images/logo (1).png" alt="">
    <img height="28" src="@/assets/images/logo-text.png" alt="">
    <div class="header-right">
      <img height="12" src="@/assets/images/school-logo-text.png" alt="">
      <img height="42" src="@/assets/images/school-logo.png" alt="">
    </div>
  </div>
</template>


<style scoped>
*{
  padding: 0;
  margin: 0;
}
.header{
  padding: 10px 20px;
  display: flex;
  width: 100%;
  height: 10%;
  background: transparent;
  align-items: center;
}
.header-right{
  display: flex;
  width: 10px;
  height: 100%;
  flex-grow: 1;
  justify-content: right;
  align-items: center;
  gap: 15px;
}
</style>