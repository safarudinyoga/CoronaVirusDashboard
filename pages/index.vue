<template>
  <div class="container">
    <div class="one">
      1
    </div>
    <div class="two">
      2
    </div>
    <div class="three">
      3
    </div>
    <div class="four">
      4
    </div>
    <div class="five">
      5
    </div>
    <div class="six">
      6
    </div>
    <div class="seven">
      7
    </div>
    <div class="eight">
      8
    </div>
    <div class="nine">
      9
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
  // grid-template-areas: "one two three four";

  div {
    background-color: aqua;
    text-align: center;
    // padding: 30px;
  }
}

// .one {
//   grid-area: one;
// }
// .two {
//   grid-area: two;
// }
// .three {
//   grid-area: three;
// }
// .four {
//   grid-area: four;
// }
// .five {
//   grid-area: five;
// }
// .six {
//   grid-area: six;
// }
// .seven {
//   grid-area: seven;
// }
// .eight {
//   grid-area: eight;
// }
// .nine {
//   grid-area: nine;
// }

</style>
