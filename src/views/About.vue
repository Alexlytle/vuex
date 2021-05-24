<template>
  <div class="about">
    <img alt="Vue logo" src="../assets/logo.png">
    <h1>about</h1>
    <div class="counter">
      {{$store.state.counter}}
    </div>
    <div class="buttons">
          <button @click = "$store.dispatch('decreaseCounter')" >-</button>
          <button @click = "$store.dispatch('increaseCounter')" >+</button>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src


export default {
  name: 'About',
 

 
}
</script>
<style>
  div{
    margin-bottom: 20px;
  }
  .counter{
    font-size: 80px;
  }
  .buttons button{
    font-size: 40px;
    width: 100px;
    margin: 0 10px;

  }
</style>
