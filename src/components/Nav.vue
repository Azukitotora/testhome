<template>
  <div>
    <a href="#" class="nav-button" @click="clickSmoothScroll('#about')">About</a>
    <a href="#" class="nav-button" @click="clickSmoothScroll('#contact')">Contact</a>
    <a href="#" class="nav-button" @click="clickSmoothScroll('#function')">Function</a>
    <a href="#" class="nav-button" @click="clickSmoothScroll('#cv')">CV</a>
    <a href="#" class="nav-button" @click="clickSmoothScroll('#interest')">Interest</a>
  </div>
</template>


<script>
export default {
  methods: {
    clickSmoothScroll (x) {
      event.preventDefault()
      this.$SmoothScroll(
        document.querySelector(x),
        800,
        null,
        null,
        'y'
      )
    }
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Antic+Slab&display=swap');

.nav-button{
  padding:10px;
  text-decoration: none;
  border-radius: 5px;
  margin-right:10px;
  margin-left: 10px;
  outline: none;
  color:cadetblue;
  font-family: 'Antic Slab', serif;
}
</style>