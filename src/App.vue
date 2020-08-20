<template>
  <div id = "main">
    <Header id = "header"></Header>
    <div class = "nav-res">
      <a href="#" class="link-content" @click="clickSmoothScroll('#about')">
        <p class="comment">About</p>
      </a>
      <a href="#" class="link-content" @click="clickSmoothScroll('#contact')">
        <p class="comment">Contact</p>
      </a>
      <a href="#" class="link-content" @click="clickSmoothScroll('#function')">
        <p class="comment">Function</p>
      </a>
      <a href="#" class="link-content" @click="clickSmoothScroll('#cv')">
        <p class="comment">CV</p>
      </a>
      <a href="#" class="link-content" @click="clickSmoothScroll('#interest')">
        <p class="comment">Interest</p>
      </a>
    </div>
    <div>
      <About id="about"></About>
      <Contact id="contact"></Contact>
      <Function id="function"></Function>
      <CV id="cv"></CV>
      <Interest id="interest"></Interest>
    </div>
  </div>
</template>

<script>
import 'normalize.css'
import Header from './components/header.vue'
import About from './components/about.vue'
import Contact from './components/contact.vue'
import Function from './components/function.vue'
import CV from './components/cv.vue'
import Interest from './components/interest.vue'
import '@fortawesome/fontawesome-free/js/fontawesome';
import '@fortawesome/fontawesome-free/js/solid';
import '@fortawesome/fontawesome-free/js/regular';

//export defaultで他のファイルから関数、オブジェクト、プリミティブを手に入れる
export default {
  name: 'main',
  components: {
    Header,
    About,
    Contact,
    Function,
    CV,
    Interest
  },
  methods:{
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
.nav-res{
  display: none;
}
</style>