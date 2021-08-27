<template>


<section class="hero is-link is-fullheight">
  <div class="hero-body">
    <div class="">
            <p class="title has-text-centered">
              Knit Counter
            </p>
      <p class="title has-text-centered">
        {{counter}}
      </p>
      <p class="subtitle">
        <b-button type="is-success" @click="counter++">Increase</b-button>
      <b-button type="is-danger" @click="counter--">Decrease</b-button>     
      </p>
    </div>
  </div>
  
  
  
</section>


</template>

<script>
export default {
  data () {
    return {
      counter: 0,
      items: [
        {
          title: 'Home',
          icon: 'home',
          to: { name: 'index' }
        },
        {
          title: 'Inspire',
          icon: 'lightbulb',
          to: { name: 'inspire' }
        }
      ]
    }
  }
}
</script>

<style>

</style>