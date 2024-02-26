<template>
  <div id="app">

    <transition>
      <router-view />
    </transition>
  </div>
</template>

<style>
@import url('https://cdn.bootcss.com/font-awesome/4.7.0/css/font-awesome.css');

* {
  margin: 0;
  padding: 0;
}
a {
  text-decoration: inherit;
}
ul,
ol {
  list-style: none;
}
h1,
h2,
h3,
h4 {
  font: inherit;
}
input,
select,
button {
  font: inherit;
}
html,
body {
  height: 100%;
  -webkit-user-select: none;
  -webkit-touch-callout: none;
  -webkit-tap-highlight-color: transparent;
}
body {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen,
    Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
}
#app {
  height: 100%;
  overflow: hidden;
}




  @keyframes blurAnimation {
        0% {
            filter: blur(20px); 
        }
        90% {
            filter: blur(2px); 
        }
        100% {
            filter: blur(0px); 
        }
    }

    body {
        animation-name: blurAnimation; 
        animation-duration: 5s; 
        animation-fill-mode: forwards;
        position: relative; 
    }


    .loading-overlay {
        position: absolute; 
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background-color: rgba(255, 255, 255, 0.8);
        display: flex;
        justify-content: center;
        align-items: center;
        z-index: 999; 
        display: none; 
    }

    .loading-overlay p {
        font-size: 24px;
        color: #333;
    }

</style>
