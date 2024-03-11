<template>
  <video controls>
    <source src="@/assets/images/PeetersThomasThisIsMe.mp4" type="video/mp4">

  </video>
  <video controls>
    <source src="@/assets/images/PeetersThomasDynamicMachine.mp4" type="video/mp4">
  </video>

</template>

<script>
export default {
  name: "3dProjectView"
}
</script>

<style scoped>
video{
  width: 50%;
  height: 50%;
}
</style>