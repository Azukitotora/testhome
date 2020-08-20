
<template>
  <div class="header">
    <div class="header-inner">
      <h1 class="title">AOC</h1>
      <Nav class="nav"></Nav>
    </div>
  </div>
</template>

<script>
import Nav from './Nav.vue'
export default{
    components:{
        Nav
    }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Comic+Neue:wght@300&display=swap');

.header{
  background-color:white;
  position: sticky;
  top: 0;
  width: 100%;
  z-index: 1;
}
.header-inner{
  margin-left: 5%;
  margin-right: 5%;
  display: flex;
}
.title{
  font-family: 'Comic Neue', cursive;
  padding:20px 0px;
  margin:unset;
  color:cadetblue;
}
.nav{
  margin: auto ;
  margin-right: 0;
  padding: auto;
}
</style>