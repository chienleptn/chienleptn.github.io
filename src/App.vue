<template>
  <div id="app">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@500;600;700;900&amp;display=swap" rel="stylesheet">
    <script type="module" src="https://unpkg.com/ionicons@5.0.0/dist/ionicons/ionicons.esm.js"></script>
    <Index />
  </div>
</template>

<script>
import Index from './components/Index.vue'

export default {
  name: 'App',
  components: {
    Index
  }
}
</script>

<style>
#app {
  color: #2c3e50; 
}
@-ms-viewport {
		width: device-width;
}

.yellow {
  color: #fcc419;
}

.maincolor {
  color: #2c3e50; 
}

body {
  -ms-overflow-style: scrollbar;
  font-family: "Poppins", sans-serif;
  background: #f1f3f5;
  widows: 100%;
  width: 100%;
  overflow-x: hidden;
}

@media screen and (max-width: 360px) {

  html, body {
    min-width: 320px;
  }

}

html {
  box-sizing: border-box;
}

*, *:before, *:after {
  box-sizing: inherit;
}
</style>
