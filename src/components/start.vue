<template>
  <div class="container relative">
    <div class="card">
      <img class="image" src="static/bohoturtle.svg">
    </div>
    <div @mouseover="dostuff"  class="bottom note absolute">
      <p>SVG can swim</p>
    </div>
  </div>
</template>

<script>
  var moveTurtle = function(){
    TweenMax.to(jQuery('.image'),1,{opacity:0})
  }
  export default {
    name: 'test',
    methods:{
      dostuff : function(){
        console.log("HELLO");
        moveTurtle();
      },
      // moveTurtle : function(){
      // }
    }
  }


</script>
<style>
  .card{
    max-width: 800px;
    padding:0 20px;
  }
  .image{
    width:100%;
    height: 100vh;
  }
  .note{
    max-width: 200px;
    text-center:center;
    padding: 0 20px;
    border: 2px black double;
    transition:all 1s ease-out;
  }
  .note:hover{
    transform:translateX(30px);
    opacity: 0;
  }
  .note >  p{
    font-family: Helvetica;
    font-size:14px;
  }
  .bottom{
    bottom:20%;
    right:10%;
  }
</style>

