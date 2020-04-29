<template>
  <div class="container">
    <div class="navbar">
      navbar
      <nav>
        <ul>
          <li>
            <h1>icon</h1>
          </li>
          <li>
            <h1>icon</h1>
          </li>
          <li>
            <h1>icon</h1>
          </li>
          <li>
            <h1>icon</h1>
          </li>
          <li>
            <h1>icon</h1>
          </li>
        </ul>
      </nav>
    </div>
    <div class="logos">
      logo
      <nav>
        <ul>
          <li>
            <h1>icon</h1>
          </li>
          <li>
            <h1>icon</h1>
          </li>
          <li>
            <h1>icon</h1>
          </li>
        </ul>
      </nav>
    </div>
    <div class="content">
      <h3>coronavirus</h3>
      <h1>covid-19</h1>
      <h4>Coronavirus disease (COVID-19) is an infectious disease caused by a newly discovered coronavirus. Most people infected with the COVID-19 virus will experience mild to moderate resporatory illness and recover without requiring special treatment...</h4>
      <div />
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

  div {
    background-color: aqua;
  }
}

.navbar {
  grid-column: 1/7;

  li {
  list-style-type: none;
  margin: 0 25px;
  }

  nav {
  width: 100%;
  }

  ul {
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: center;
  }
}

.logos {
  grid-column: 10/13;

  li {
  list-style-type: none;
  margin: 0 15px;
  }

  nav {
  width: 100%;
  }

  ul {
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: center;
  }
}

.content {
  grid-column: 1/7;
  grid-row: 2/5;
  h1 {
    text-transform: uppercase;
    color: #be4848;
    font-weight: bolder;
    letter-spacing: 2px;
  }
  h3 {
    text-transform: uppercase;
    letter-spacing: -1px;
  }
  div {
    width: 30px;
  }
}

.maps {
  grid-column: 1/5;
  grid-row: 5/7;
}

.background {
  grid-column: 7/10;
  grid-row: 1/7;
}

h1 {
  font-size: 50px;
}
h2 {
  font-size: 24px;
}
h3 {
  font-size: 20px;
}
h4 {
  font-size: 16px;
}
h5 {
  font-size: 18px;
}
h6 {
  font-size: 12px;
}

h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: 'Ubuntu', sans-serif;;
  margin: 0px auto;
}
</style>
