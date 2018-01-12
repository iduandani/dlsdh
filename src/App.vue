<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style>
@font-face {
  font-family: 'iconfont';  /* project id 536546 */
  src: url('//at.alicdn.com/t/font_536546_un6mpiksb6mkj4i.eot');
  src: url('//at.alicdn.com/t/font_536546_un6mpiksb6mkj4i.eot?#iefix') format('embedded-opentype'),
  url('//at.alicdn.com/t/font_536546_un6mpiksb6mkj4i.woff') format('woff'),
  url('//at.alicdn.com/t/font_536546_un6mpiksb6mkj4i.ttf') format('truetype'),
  url('//at.alicdn.com/t/font_536546_un6mpiksb6mkj4i.svg#iconfont') format('svg');
}
.iconfont {
  font-family:"iconfont" !important;
  font-size:16px;
  font-style:normal;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

.icon-sou:before { content: "\e631"; }

.icon-down-trangle:before { content: "\e600"; }
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  height: 100%;
  box-sizing: border-box;
}
body,html{
  height: 100%;
  overflow: auto;
  box-sizing: border-box;
}
*{
  padding: 0;
  margin: 0;
}
</style>
