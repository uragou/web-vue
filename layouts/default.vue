<template>
  <div id="app">
    <humber/>
    <transition name="page" mode="out-in">
      <nuxt/> 
    </transition>
  </div>
</template>

<script>
import Humber from '~/components/Humber.vue'

export default {
  components:{
    Humber
  }
}
</script>


<style>
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
  text-align: center;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
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

.page-enter-active {
  transition: all 22s;
  opacity: 1;
}
.page-leave-active {
  transition-property: all;
  transition-duration: 8s;
  opacity: 1;
}

.page-enter{
  opacity: 0;
}
.page-leave{
  opacity: 1;
}
.page-leave-to{
  opacity: 0;
}
</style>
