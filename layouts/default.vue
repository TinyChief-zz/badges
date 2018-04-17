<template>
  <div class="container">
    <header>
      <div>
        <h1>Site name</h1>
      </div>
      <nav>
        <ul>
          <nuxt-link to="/"><li><a class="nav-link" href="#">Главная</a></li></nuxt-link>
          <nuxt-link to="/galery"><li><a class="nav-link" href="#">Галерея</a></li></nuxt-link>
          <nuxt-link to="/users"><li><a class="nav-link" href="#">Участники</a></li></nuxt-link>
          <nuxt-link to="/contact"><li><a class="nav-link" href="#">Связаться</a></li></nuxt-link>
        </ul>
      </nav>
    </header>
    <nuxt/>
  </div>
</template>

<script>

</script>

<style>
html
{
  font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  background-color: #fffcf0;
}
*, *:before, *:after
{
  box-sizing: border-box;
  margin: 0;
}
li {
  list-style: none
}
a {
  text-decoration: none;
  color: black;
}
.container
{
  max-width: 960px;
  margin: 0 auto;
  min-height: 100vh;
  background-color: #f15c5c;
}
section {
  padding: 10px 15px;
  display: flex;
  flex-flow: column;
  align-items: center;
}
.section-title {
  margin-bottom: 15px;
  color: #F8FAFF;
  position: relative;
  display: inline-block;
  line-height: 1.6;
  width: 400px;
  /*text-align: center;*/
}
.section-title::after, .section-title::before {
  content: "";
  position: absolute;
  height: 4px;
  width: 100%;
  background-color: #f8faff;
  transition: 0.4s all ease;
  transform-origin: 0% 50%;
}
.section-title::after {
  transform: rotate(180deg) translateX(-400px);
}
.section-title h1 {
  text-align: center;
}
section:hover .section-title::after {
  height: 1px;
  width: 0;
}
section:hover .section-title::before {
  width: 0;
  height: 1px;
}

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px 15px;
  border-bottom: 3px solid #492540;
  color: #F8FAFF;
}
nav ul {
  display: flex;
}
.nav-link {
  color:#F8FAFF;
  font-weight: bold;
  margin: 0px 7px;
  padding: 10px 18px;
  border-radius: 8px;
  border: 1px dashed transparent;
  transition: 0.2s background-color linear;
}
.nav-link:hover {
  background-color: #fff;
  color: #34314c;
  border: 1px dashed #34314c;
}



</style>
