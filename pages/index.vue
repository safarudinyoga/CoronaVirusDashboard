<template>
  <div class="container">
    <div class="navbar">
      navbar
    </div>
    <div class="logos">
      logo
    </div>
    <div class="content">
      content
    </div>
    <div class="maps">
      earth logo
    </div>
    <div class="background">
      5
    </div>
  </div>
</template>

<script>

export default {
}
</script>

<style lang="scss" scoped>
.container {
  // width: 1366px;
  // height: 768px;
  max-width: 960px;
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  // grid-template-rows: auto;
  grid-auto-rows: minmax(100px, auto);
  gap: 10px;
  margin: 0 auto;
  // grid-template-areas: "one two three maps";

  div {
    background-color: aqua;
    text-align: center;
    // padding: 30px;
  }
}

.navbar {
  grid-column: 1/7;
}
.logos {
  grid-column: 10/13;
}
.content {
  grid-column: 1/7;
  grid-row: 2/5
}
.maps {
  grid-column: 1/5;
  grid-row: 5/7;
}
.background {
  grid-column: 7/10;
  grid-row: 1/7;
}

</style>
