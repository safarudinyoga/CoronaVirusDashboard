<template>
  <div class="container background">
    <div class="navbar">
      <nav>
        <ul>
          <li>
            <img class="virus" :src="virussvg" alt="">
          </li>
          <li>
            <h4>about</h4>
          </li>
          <li>
            <h4>news</h4>
          </li>
          <li>
            <h4>catalog</h4>
          </li>
          <li>
            <h4>contacts</h4>
          </li>
        </ul>
      </nav>
    </div>
    <div class="content">
      <h3>coronavirus</h3>
      <h1>covid-19</h1>
      <h4>Coronavirus disease (COVID-19) is an infectious disease caused by a newly discovered coronavirus. Most people infected with the COVID-19 virus will experience mild to moderate resporatory illness and recover without requiring special treatment...</h4>
      <div class="see-more">
        <div class="box-arrow-outside">
          <div class="box-arrow">
            <div class="long-arrow-right" />
          </div>
        </div>
        <div class="texting">
          <h3>See More</h3>
        </div>
      </div>
    </div>
    <div class="maps">
      <img :src="mapcorona" alt="">
    </div>
    <div class="dots">
      <div class="halfdot" />
    </div>
    <div class="full">
      <div class="fulldot" />
      <div class="logos">
        <nav>
          <ul>
            <li>
              <img :src="instagramsvg" alt="">
            </li>
            <li>
              <img :src="githubsvg" alt="">
            </li>
            <li>
              <img :src="linkedinsvg" alt="">
            </li>
          </ul>
        </nav>
      </div>
    </div>
  </div>
</template>

<script>
import instagramsvg from '~/assets/brands-and-logotypes.svg'
import githubsvg from '~/assets/shape.svg'
import virussvg from '~/assets/virus.svg'
import linkedinsvg from '~/assets/social-media.svg'
import mapcorona from '~/assets/worldmap.png'

export default {
  data () {
    return {
      instagramsvg,
      githubsvg,
      virussvg,
      linkedinsvg,
      mapcorona
    }
  }
}
</script>

<style lang="scss" scoped>
.container {
  width: 1366px;
  height: 768px;
  // max-width: 1920px;
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  // grid-template-rows: auto;
  grid-auto-rows: minmax(100px, auto);
  gap: 10px;
  margin: 0 auto;
}

.navbar {
  grid-column: 1/7;

  li {
  list-style-type: none;
  margin: 0 20px;
  }

  nav {
  width: 100%;
  height: 100%;
  }

  ul {
  margin-top: 30px;
  margin-left: 30px;
  padding: 0;
  display: flex;
  align-items: center;
  }

  h4 {
    text-transform: uppercase;
    color: white;
  }
}

.content {
  grid-column: 1/7;
  grid-row: 2/5;

  margin-left: 50px;
  display: flex;
  flex-direction: column;
  justify-content: center;

  h1 {
    text-transform: uppercase;
    margin: 0;
    color: #db3b3b;
    letter-spacing: 5px;
    font-family: fantasy;
    font-size: 90px;
  }
  h3 {
    text-transform: uppercase;
    font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
    color: white;
    margin: 0;
  }
  h4 {
    color: #b6b6b6;
    text-align: justify;
    margin: 0;
    width: 400px;
  }

  .see-more {
  width: 300px;
  height: 100px;
  margin-top: 10px;
  display: flex;
  justify-content: flex-start;
  align-items: center;

    h3 {
      margin: 0 30px;
      text-transform: none !important;
    }

    .box-arrow-outside {
    width: 80px;
    height: 80px;
    background-color: #171314;
    border-radius: 50%;
    border: 2px solid #474747;
    position: relative;

      .box-arrow {
        width: 50px;
        height: 50px;
        background-color: #53201f;
        border-radius: 50%;
        border: 2px solid #5b5b5b;
        position: relative;
        top: 13px;
        left: 12.5px;

        .long-arrow-right {
          display: block;
          margin: 0;
          width: 10px;
          height: 10px;
          border-top: 2px solid white;
          border-left: 2px solid white;
          transform: rotate(135deg);
          position: absolute;
          top: 18px;
          left: 20px;

          &::after {
            content: "";
            display: block;
            width: 2px;
            height: 15px;
            background-color: white;
            transform: rotate(-45deg) translate(4.5px, 1px);
            left: 0;
            top: 0;
          }
        }
      }
    }
  }
}

.maps {
  grid-column: 1/5;
  grid-row: 5/7;
  display: flex;

  img {
    align-self: flex-start;
    width: 430px;
    height: 200px;
    object-fit: contain;
    }
}

.dots {
  grid-column: 5/7;
  grid-row: 5/7;

  $size: 110px;
  display: flex;

  .halfdot {
  height: $size;
  width: $size * 2;
  border-top-left-radius: $size * 2;
  border-top-right-radius: $size * 2;
  align-self: flex-end;
  background-image: linear-gradient(to right, #da3a3a, #76191b);
  }
}

.backcontent {
  grid-column: 7/10;
  grid-row: 1/7;
}

.full {
  grid-column: 7/13;
  grid-row: 1/7;
  display: flex;
  position: relative;

  .fulldot {
  $size: 630px;
  height: $size;
  width: $size;
  border-radius: 50%;
  align-self: center;
  background-image: linear-gradient(to right, #da3a3a, #76191b);

    img {
    width: 800px;
    height: 800px;
    }
  }

  .logos {
    position: absolute;
    top: 20px;
    right: 30px;

    li {
    list-style-type: none;
    margin: 0 15px;
    }

    nav {
    width: 200px;
    }

    ul {
    margin-top: 25px;
    padding: 0;
    display: flex;
    justify-content: center;
    }

    img {
    width: 30px;
    height: 30px;
    object-fit: contain;
    }
  }
}
</style>
