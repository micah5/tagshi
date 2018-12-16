<template>
  <div class="hello"><!-- <g class="rellax" data-rellax-speed="3"> :data-rellax-speed="width > 900 ? 1.3 : 1.3" -->
    <img src="../assets/logo.svg" style="width: 40vh; position: absolute; left: 15%; top: 8vh;"></img>
    <div class="text">
      sorry, we aren’t ready yet<br>
      in the mean time you can check out
      <div class="parent">
        <div class="column"><a href="https://drive.google.com/file/d/1CWKItDnbaESeofD_6WJtgrx9JDd3NJog/view?usp=sharing">our deck</a></div>
        <div class="column"><a href="https://www.youtube.com/watch?v=rGJPMh1LJTE">a demo</a></div>
        <div class="column"><a href="https://angel.co/tagshi">angel.co</a></div>
        <div class="column"><a href="mailto:98mprice@gmail.com">email us</a></div>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'HelloWorld',
  props: {
    msg: String,
  },
  data() {
    return {
      width: 0,
    }
  },
  mounted: function() {
    this.width = window.innerWidth
    console.log(this.width)
  }
}
</script>

<style scoped>
@font-face {
    font-family: 'ArcaMajora3-Bold';
    src: url('../assets/fonts/ArcaMajora3-Bold.eot'), url('../assets/fonts/ArcaMajora3-Bold.woff') format('woff');
    font-weight: normal;
    font-style: normal;
}

.text {
  position: absolute;
  top: 85%;
  left: 50%;
  margin-right: -50%;
  transform: translate(-50%, -50%);
  font-family:'ArcaMajora3-Bold';
  font-size: 3vw;
  color: #1C2541;
  letter-spacing: -1px;
  text-align: center;
  width: 80%;
}
.parent {
  display: flex;
  flex-direction:row;
  margin-top: 1rem;
}
.column {
  flex: 1 1 0px;
}
@media only screen and (max-width: 600px) {
  .text {
    font-size: 5vw;
    width: 100%;
  }
}
a {
  color: #3A506B;
  transition: 0.1s linear all;
  cursor: pointer;
  text-decoration: none;
}
a:hover {
  color: white;
}
</style>
