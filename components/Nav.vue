<template>
  <div class="nav">
    <div class="nav-logo">
      <div>SR</div>
    </div>
    <div class="nav-links">
      <div>BLOG</div>
      <div>PROJECTS</div>
      <div>CONTACT</div>
    </div>
    <div class="nav-search">
      <div>Search</div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.nav {
  display: flex;
  font-family: 'Montserrat';
  height: 70px;
}

.nav-logo {
  background-color: #faefc1;
  align-items: center;
  color: rgb(41, 44, 44);
  display: flex;
  font-family: 'Lora';
  font-size: 3em;
  font-weight: 500;
  justify-content: center;
  letter-spacing: -0.09em;
  width: 15vw;
}

.nav-links {
  align-items: center;
  background-color: #e0e4cf;
  display: flex;
  font-weight: 600;
  justify-content: space-between;
  padding: 0 20px;
  width: 70vw;
}

.nav-search {
  background-color: palevioletred;
  align-items: center;
  display: flex;
  font-family: 'Lora';
  font-size: 1.5em;
  justify-content: center;
  width: 15vw;
}
</style>