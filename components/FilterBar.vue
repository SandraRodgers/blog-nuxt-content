<template>
  <div class="filterbar">
    <div class="filterbar-links">
      <div>ALL</div>
      <div>WEBDEV</div>
      <div>FOODIE</div>
      <div>LIFE</div>
      <div>MUSINGS</div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.filterbar {
  display: flex;
  font-family: 'Montserrat';
  height: 70px;
}

.filterbar-links {
  align-items: center;
  background-color: #e0e4cf;
  display: flex;
  font-weight: bold;
  justify-content: center;
  padding: 0 20px;
  width: 100vw;
}

.filterbar-links > div {
  padding: 0 8px;
}
</style>