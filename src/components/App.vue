<template>
  <div id="app">

      <test></test>

  </div>
</template>
<!-- App -->


<script>
  import test from './start.vue'

  export default {
    name: 'app',
    components: {
      test,
    }
  }
</script>

<!-- CSS libraries -->
<style src="normalize.css/normalize.css"></style>

<!-- Global CSS -->
<style>
  code {
    font-family: Menlo, Monaco, Lucida Console, Liberation Mono, DejaVu Sans Mono, Bitstream Vera Sans Mono, Courier New, monospace, serif;
    font-size: 0.9em;
    white-space: pre-wrap;
    color: #2c3e50;
  }

  code::before, code::after {
    content: '`';
  }
</style>

<!-- Scoped component css -->
<!-- It only affect current component -->
<style>
  /*UTILITY CSS */
  .container {
    text-align: center;
    margin:auto;
    max-width: 1000px;
  }
  .relative{
    position: relative;
  }
  .absolute{
    position: absolute;
  }
  .center{
    margin:auto;
  }


  /*.logo {*/
    /*animation: spin 4s 1s infinite linear*/
  /*}*/

  /*@keyframes spin {*/
    /*from {transform:rotate(0deg);}*/
    /*to {transform:rotate(360deg);}*/
  /*}*/
</style>
