<template>
  <div>
    <div class="bg-image"></div>
    <el-container class="main-container">
      <el-header class="header">
        <el-row>
          <el-col :span="20" :offset="2">
            <el-row type="flex" justify="space-between">
              <el-col :xs="24" :sm="4">
                <img class="logo" src="~/assets/bm-texture.png" alt="Logo">
              </el-col>
              <el-col :xs="24" :sm="18" class="menu-container">
                <el-menu class="menu" mode="horizontal">
                  <el-menu-item index="1">Home</el-menu-item>
                  <el-menu-item index="2">Videos</el-menu-item>
                  <el-menu-item index="3">Tour</el-menu-item>
                  <el-menu-item index="4">Sakura Gakuin</el-menu-item>
                  <el-menu-item index="5">Contact</el-menu-item>
                </el-menu>
              </el-col>
            </el-row>
          </el-col>
        </el-row>
      </el-header>
      <el-main>
        <nuxt/>
      </el-main>
    </el-container>
  </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css?family=Averia+Serif+Libre:400,700');

*, *:before, *:after {
  box-sizing: border-box;
  margin: 0;
}

html {
  font-family: sans-serif;
  font-size: 16px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  box-sizing: border-box;
}

body {
  min-height: 100vh;
  background-color: #000;
}

.bg-image {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: url('/fox-left.png'), url('/fox-right.png');
  background-repeat: no-repeat, no-repeat;
  background-position: left 80px,right 80px;
  background-size: auto 100%;
}

.main-container {
  position: relative;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}

.header, .menu, .menu li:hover, .menu li:focus {
  background-color: #000 !important;
}

.header {
  padding-top: 15px;
  margin-bottom: 10px;
}

.logo {
  width: 110px;
  padding-top: 7px;
}
.menu-container {
  display: flex;
  justify-content: flex-end;
}

.el-menu--horizontal {
  border-bottom: 0;
}

.menu li {
  font-family: 'Averia Serif Libre', cursive;
  color: #fff !important;
  font-size: 15px;
}

.el-menu--horizontal>.el-menu-item.is-active {
  border-bottom: 2px solid #ffffff;
}
</style>

