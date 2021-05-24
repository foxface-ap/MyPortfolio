<template>
<div id="Nav">
<div class="navbar">
        <a href="#sec-1">About</a>
        <a href="#sec-2">Experience</a>
        <a href="#sec-3">Projects</a>
      </div>
</div>
</template>

<script>

export default {
  name: 'app',
  components: { 
  }
}
</script>

<style scopped>

.navbar {
  overflow: hidden;
  background-color: #006182;
  position: fixed;
  top: 0;
  width: 100%;
  height: 60px;
  border-radius: 0px;
  z-index: 9999;
}

.navbar a {
  float: left;
  display: block;
  color: #f2f2f2;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 17px;
  width: 30%;
  
}

.navbar a:hover {
  background: #006182;
  color: #001b24;
}

</style>
