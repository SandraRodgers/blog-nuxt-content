<template>
  <section class="masthead" role="img" aria-label="Image Description">
    <h1>Sandra Rodgers</h1>
    <h2>FRONT END DEVELOPER</h2>
  </section>
</template>

<script>
export default {}
</script>

<style scoped>
.masthead {
  align-items: center;
  background-size: cover !important;
  background: linear-gradient(
      to bottom,
      rgba(0, 0, 0, 0) 0%,
      rgba(0, 0, 0, 0) 0%,
      rgba(245, 138, 138, 0.35) 100%
    ),
    url('~assets/pink_background.jpeg') no-repeat center center scroll;
  display: flex;
  flex-direction: column;
  font-family: 'Merriweather';
  justify-content: center;
  height: 70vh; /* if you don't want it to take up the full screen, reduce this number */
  overflow: hidden;
  text-align: center;
  /* width: 100%; */
}

h1 {
  font-style: normal;
  /* font-weight: bold; */
  color: whitesmoke;
  font-size: 11vmin;
  letter-spacing: 0.03em;
  line-height: 1;
  /* text-shadow: 1px 1px 4px rgb(0, 175, 169); */
  margin-bottom: 40px;
}

h2 {
  font-family: 'Montserrat';
  color: rgb(42, 56, 56);
}
</style>