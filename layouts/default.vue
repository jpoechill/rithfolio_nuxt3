<template>
  <div>
    <div class="w-100 custom-gradient border-bottom">
      <div class="container">
        <div class="row">
          <div class="py-4" />
        </div>
      </div>
    </div>

    <div class="w-100 sticky top-0 pb-0 z-10"
      style="background-color: #FFF; box-shadow: 0 .5rem 1rem rgba(0,0,0,.01)!important;">
      <!-- Mobile -->
      <div class="container md:hidden">
        <div class="row sticky top-0">
          <div class="columns-12md bg-white py-0 border-left border-right text-center px-4">
            <!-- content -->asdas
            <div class="flex justify-between">
              <div class="border-right py-3 pr-3">
                <span class="font-weight-bold">
                  <nuxt-link to="/">Po Rith</nuxt-link>
                </span> |
                <span>
                  Typescript x Design Mobile
                </span>
              </div>
              <div class="py-3" style="width: 44%;">
                <img src="/squiggle.svg" class="w-100" alt="" />
              </div>
              <span class="font-weight-bold pl-3 py-3 border-left">
                <nuxt-link to="/">CV</nuxt-link>
              </span>
            </div>
          </div>
        </div>
      </div>

      <!-- Desktop -->
      <div class="container mx-auto text-center">
        <div class="grid grid-cols-12 w-100">
          <div class="col-span-5 border-l border-r py-3">
            <img src="/self_bw.jpg" class="w-[32px] inline border rounded-full mr-4" alt="avatar">
            <span class="font-bold inline">
              <nuxt-link to="/">Po Rith</nuxt-link>
            </span> | Typescript x Design
          </div>
          <div class="col-span-5 border-r py-4">
            <img src="/squiggle.svg" class="mx-auto" alt="">
          </div>
          <div class="col-span-2 border-r py-3">
            <span class="font-bold">
              <a href="/prith_resume_041922.pdf" target="new">CV</a>
            </span>
          </div>
        </div>
      </div>
    </div>


    <div class="w-100 border-b" style="background-color: #FFF;">
      <div class="sticky top-[55px]  linear-gradient border-b border-t w-100 z-10 py-2 mx-auto bg-white">
        <div class="row pt-0 my-1 pb-0">
          <div class="col-md-12 text-center">
            <h5 class="pb-0 mb-0 font-medium text-md px-5 text-gray-600">
              Recent Projects
            </h5>
          </div>
        </div>
      </div>
      <slot />
    </div>

    <div class="">
      <div class=" container py-10 mx-auto">
        <div class="grid grid-cols-12">
          <div class="col-span-1 col-start-3 p-5 pt-7">
            <div class="px-5 md:px-0">
              <img src="/self_bw.jpg" class="w-full rounded-full" alt="avatar">
            </div>
          </div>
          <div class="md:col-span-7 p-7">
            <p class="">
              Greetings! I'm Po, and I specialize in building robust web applications with <i>Vue.js</i>. <br>
              If you are interested in learning more, please feel free to get in touch!<br>
            </p>
            <div class="text-left">
              ~ <a href="mailto:heys@rithfolio.com">Email</a>,
              <a href="https://github.com/jpoechill" target="_blank">Github</a>,
              <a href="https://www.notion.so/posblog/Po-s-Technology-Blog-d5360cafbfb046d8957bf6b456a4e75d"
                target="_blank">Blog</a>,
              <a href="https://linkedin.com/in/porith" target="_blank">LinkedIn</a>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="w-100 py-4 bg-white border-t">
      <div class="container mx-auto text-center">
        <!-- Mobile -->
        <div class="row md:hidden">
          <div class="col-md-6 py-2">
            <span class="text-muted">
              <small><em>
                  Hashtags: #Algorithms, #JavaScript, #Design, #Vue.js, #HTML/CSS, #Git
                </em></small><br>
              <small class="text-muted mt-2 d-block">
                Proudly made with <a href="https://github.com/vuejs/vue" target="_blank" class="vue-link">Vue.js</a>. ©
                2023
              </small>
            </span>
          </div>
        </div>

        <!-- Desktop -->
        <div class="grid grid-cols-12 w-100">
          <div class="col-span-6 text-left py-2">
            <span class="text-muted">
              <small><em>
                  Hashtags: #Algorithms, #JavaScript, #Design, #Vue.js, #HTML/CSS, #dysonspheres
                </em></small>
            </span>
          </div>

          <div class="col-span-6 text-right py-2">
            <small class="text-muted">
              Proudly made with <a href="https://github.com/vuejs/vue" target="_blank" class="vue-link">Vue.js</a>. ©
              2023
            </small>
          </div>
        </div>
      </div>
    </div>


  </div>
</template>

<script>
</script>

<style>
body,
html {
  font-size: 16px;
  height: 100%;
}

body {
  color: #333;
  background-color: #f7f7f7 !important;
}

.vue-link {
  color: teal;
}

.custom-gradient {
  background: linear-gradient(215deg, #ff0000, #feff00, #6bff00, #00ffe6, #0100ff, #cc00ff, #ff0000);
  background-size: 1400% 1400%;

  -webkit-animation: AnimationName 120s ease infinite;
  -moz-animation: AnimationName 120s ease infinite;
  animation: AnimationName 120s ease infinite;
}

@-webkit-keyframes AnimationName {
  0% {
    background-position: 0% 51%
  }

  50% {
    background-position: 100% 50%
  }

  100% {
    background-position: 0% 51%
  }
}

@-moz-keyframes AnimationName {
  0% {
    background-position: 0% 51%
  }

  50% {
    background-position: 100% 50%
  }

  100% {
    background-position: 0% 51%
  }
}

@keyframes AnimationName {
  0% {
    background-position: 0% 51%
  }

  50% {
    background-position: 100% 50%
  }

  100% {
    background-position: 0% 51%
  }
}

.fade-enter-active,
.fade-leave-active {
  transition: opacity .2s;
}

.fade-enter,
.fade-leave-to

/* .fade-leave-active below version 2.1.8 */
  {
  opacity: 0;
}

.logo {
  min-width: 150px;
}

.special {
  font-size: 22px;
}

.weight-400 {
  font-weight: 400;
}

.weight-600 {
  font-weight: 600;
}

.active {
  padding-bottom: 2px;
  border-bottom: 3px solid #ddd;
}

.nounderline {
  text-decoration: none !important
}

@-webkit-keyframes ticker {
  0% {
    -webkit-transform: translate3d(0, 0, 0);
    transform: translate3d(0, 0, 0);
    visibility: visible;
  }

  100% {
    -webkit-transform: translate3d(-100%, 0, 0);
    transform: translate3d(-100%, 0, 0);
  }
}

@keyframes ticker {
  0% {
    -webkit-transform: translate3d(0, 0, 0);
    transform: translate3d(0, 0, 0);
    visibility: visible;
  }

  100% {
    -webkit-transform: translate3d(-100%, 0, 0);
    transform: translate3d(-100%, 0, 0);
  }
}

.ticker-wrap {
  /* position: fixed; */
  /* bottom: 0; */
  width: 100%;
  overflow: hidden;
  /* height: 4rem; */
  /* background-color: rgba(0, 0, 0, 0.9); */
  padding-left: 100%;
  box-sizing: content-box;
}

.ticker-wrap .ticker {
  display: inline-block;
  height: 4rem;
  line-height: 4rem;
  white-space: nowrap;
  padding-right: 100%;
  box-sizing: content-box;
  -webkit-animation-iteration-count: infinite;
  animation-iteration-count: infinite;
  -webkit-animation-timing-function: linear;
  animation-timing-function: linear;
  -webkit-animation-name: ticker;
  animation-name: ticker;
  -webkit-animation-duration: 30s;
  animation-duration: 30s;
}

.ticker-wrap .ticker__item {
  display: inline-block;
  padding: 0 2rem;
  /* font-size: 2rem; */
  /* color: white; */
}

@media only screen and (max-width: 600px) {
  .text-responsive {
    text-align: center !important;
  }
}

.custom-bg {
  background-color: #b7b7b70f;
  background-image: linear-gradient(135deg, #ffffff 25%, transparent 25%), linear-gradient(225deg, #ffffff 25%, transparent 25%), linear-gradient(45deg, #ffffff 25%, transparent 25%), linear-gradient(315deg, #ffffff 25%, rgb(183 183 183 / 0%) 25%);
  background-position: 40px 0, 40px 0, 0 0, 0 0;
  background-size: 80px 80px;
  background-repeat: repeat;
}

.linear-gradient {
  background: linear-gradient(#fff, #f9f9f9ee);
}

a {
  color: #007bff;
  text-decoration: none;
  background-color: transparent;
}

a:hover {
  color: #0056b3;
  text-decoration: underline;
}

.container {
  max-width: 1250px;
}
</style>