<template>
  <div id="app">
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/projects">Projects</router-link> |
      <router-link to="/contact">Contact</router-link>
    </div> -->
            <div class="header">
          <img class="circular--square" src="./assets/profile.jpg" style="width:140px;" alt="Shahibur Profile Picture">
          <h1 class="profile-name">Md. Shahibur Rahman</h1>

             <!-- <p class="status" > <strong>Open to new positions</strong></p> -->

          <div class="pure-menu pure-menu-horizontal pure-menu-scrollable">
              <ul class="pure-menu-list">

                     <li class="pure-menu-item"><a href="/" class="pure-menu-link">Home</a></li>

                    <li class="pure-menu-item"><a href="/projects" class="pure-menu-link">Projects</a></li>

                    <li class="pure-menu-item"><a href="/contact" class="pure-menu-link">Contact</a></li>


              </ul>
          </div>
        </div>
    <router-view />
  </div>
</template>

<style>
body {
padding: 20px; font-family: 'Lato', sans-serif; font-size: 16px; }
.header {text-align: center; }
.profile {width: 150px; }
.profile-name {margin-top: 5px; font-size: 25px; }
.content {max-width: 700px; margin-left: auto; margin-right: auto; }
p {font-size: 16px; line-height: 1.5; }
a {color: #258cdb; text-decoration: none; }
a:hover {color: #2571db; }
h1 {font-size: 28px; }
.ytp-chrome-top {display: none !important; }
.embed {position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; margin-bottom: 10px; margin-top: 10px; }
.embed iframe, .embed object, .embed embed {position: absolute; top: 0; left: 0; width: 100%; height: 100%; }
.circular--square {border-radius: 50%; }
.circular--square {border-top-left-radius: 50% 50%; border-top-right-radius: 50% 50%; border-bottom-right-radius: 50% 50%; border-bottom-left-radius: 50% 50%; }
#desc{text-align: justify; text-justify: inter-word; }
p.status {margin-top:0.8px; margin-bottom:0.8px;}
</style>
