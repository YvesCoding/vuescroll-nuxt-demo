<template>
  <section class="container">
      <div id="parent">
        <vue-scroll :ops="ops"> <div id="child"></div> </vue-scroll>
      </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      ops: {
        bar: {
          background: 'rgb(24, 144, 255)'
        },
        rail: {
          border: '1px solid #cecece',
          size: '20px'
        },
        scrollButton: {
          enable: true,
          background: '#cecece'
        }
      }
    }
  }
}
</script>

<style>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
#parent {
  width: 400px;
  height: 400px;
  display: inline-block;
}

#child {
  width: 800px;
  height: 800px;
  background: -webkit-linear-gradient(left top, red, blue);
  /* Safari 5.1 to 6.0 */
  background: -o-linear-gradient(bottom right, red, blue);
  /* Opera 11.1 to 12.0 */
  background: -moz-linear-gradient(bottom right, red, blue);
  /* Firefox 3.6 to 15 */
  background: linear-gradient(to bottom right, red, blue);
  /* 标准语法 */
}
</style>
