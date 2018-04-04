<template>
  <div id="app">
    <div class="wrapper">
      <div class="sidebar">
        <div class="logo">
          <a class="simple-text" href="#">
            <div class="logo-img">
              <img src="static/img/vue-logo.png" alt=""/>
            </div>
            Paper Dashboard
          </a>
        </div>
        <ul class="nav-link">
          <li><a href="#"><i class="ti-panel"></i>dashboard</a></li>
          <li><a href="#"><i class="ti-user"></i>user profile</a></li>
          <li><a href="#"><i class="ti-view-list-alt"></i>table list</a></li>
          <li><a href="#"><i class="ti-typography"></i>typography</a></li>
          <li><a href="#"><i class="ti-pencil-alt2"></i>icons</a></li>
          <li><a href="#"><i class="ti-map"></i>maps</a></li>
          <li><a href="#"><i class="ti-bell"></i>notifications</a></li>
        </ul>
        <div class="movingArrow"></div>
      </div>
      <div class="mainPanel"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
#app {
  margin: auto;
  font-size: 14px;
  font-family: 'Muli', Helvetica, Arial, sans-serif;
  box-sizing: border-box;
  color: #66615b;
  background-color: white;
}
#app a{
  font-family: 'Muli', Helvetica, Arial, sans-serif;
}
#app .sidebar {
  position: absolute;
  max-height: 100%;
  height: 100%;
  width: 259px;
  font-weight: 200;
  display: block;
  top: 0px;
  bottom: 0px;
  left: 0px;
  background-color: #212120;
}
#app .sidebar .logo {
  border-bottom: 1px solid rgba(255,255,255,0.3);
  padding: 13px 0;
  margin: 0 20px;
  box-sizing: border-box;
  width: 220px;
  height: 75px;
}
#app .sidebar .logo .simple-text {
  color: white;
  padding: 4px 0;
  font-weight: 600;
  line-height: 40px;
  text-align: left;
  background-color: transparent;
  display: block;
}
#app .sidebar .logo .simple-text .logo-img {
  background: white;
  border-radius: 50%;
  display:inline-block;
  height:40px;
  width:40px;
  text-align:center;
  margin-left: 0px;
  margin-right:10px;
}
#app .sidebar .logo .simple-text .logo-img img{
  max-width: 21px;
  vertical-align: middle;
  border: 0;
}
#app .sidebar .nav-link {
  list-style: none;
  padding-left: 0px;
  margin-bottom: 0px;
  margin-top: 0px;
}
#app .sidebar .nav-link li {
  text-transform: uppercase;
  display: block;
  box-sizing: border-box;
}
#app .sidebar .nav-link a {
  display: block;
  color: white;
  opacity: 0.7;
  margin: 10px 0px;
  padding: 10px 25px;
  box-sizing: border-box;
}
#app i{
  font-size:24px;
  float:left;
  font-weight:bold;
  margin-right: 15px;
  line-height:30px;
  height:30px;
  width:30px;
  text-align: center;
}
</style>
