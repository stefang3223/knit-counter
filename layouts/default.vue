<template>
  <div>
    

    <div class="counter-content">
      <h1>Knit Counter</h1>
      <p class="counter-val">{{counter}}</p>
      <b-button type="is-success" @click="counter++">Increase</b-button>
      <br/>
      <b-button type="is-danger" @click="counter--">Decrease</b-button>     
      <br/>
      <b-button type="is-warning" @click="counter=0">Reset</b-button>
    </div>
    
  </div>
</template>

<script>
export default {
  data () {
    return {
      counter: 0,
     
    }
  }
}
</script>

<style>
  body {
    margin: 0;
    padding: 0;
    height: 100vh;
  }
  img {
    position: fixed;
    z-index: -999;
    left: 0;
    top: 0;
    height: 100%;
    width: auto;
  }

  button {
    margin-bottom: 1rem;
    width: 10rem;
    height: 15rem;
  }

  .counter-content {
    display: block;
    height: 100%;
    width: 100%;
    
    padding: 5rem;
    margin: 0 auto;
    background-color: rgba(255,255,255,0.8);
    text-align: center;
    border-radius: 5px;
  }

  h1 {
    font-size: 2rem;
  }

  .counter-val {
    font-size: 3rem;
    text-align: center;
    font-weight: bold;
  }

</style>