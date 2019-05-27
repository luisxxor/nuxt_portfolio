<template>
  <div>
    <vuescroll :ops="ops">
      <div class="container w-screen h-screen">
        <nuxt/>
      </div>
    </vuescroll>
  </div>
</template>

<script>
import vuescroll from 'vuescroll'
export default {
  components: {
    vuescroll
  },
  data() {
    return {
      ops: {
        vuescroll: {
          mode: 'native',
          sizeStrategy: 'percent',
          wheelScrollDuration: 500
        },
        scrollPanel: {
          easing: 'easeInOutQuad'
        },
        bar: {
          background: '#F2F2F2'
        },
        rail: {},
        scrollButton: {}
      }
    }
  }
}
</script>


<style>
@import url('https://fonts.googleapis.com/css?family=Raleway&display=swap');
@import url('https://fonts.googleapis.com/css?family=Merriweather&display=swap');

html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;

  overflow: hidden;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

h1,
h2 {
  font-family: 'Raleway', sans-serif;
}

p {
  font-family: 'Merriweather', serif;
}
</style>
