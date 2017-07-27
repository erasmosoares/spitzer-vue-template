<template>
  <div class="home">
    <section class="hero">
      <div class="hero-body">
        <div class="container">
          <h1 class="title">{{ heading }}</h1>
          <div class="is-two-thirds column is-paddingless">
            <h2 class="sub is-4">{{ subheading }}</h2>
          </div>
          <a class="button is-large is-primary" id="learn">Learn more</a>
        </div>
      </div>
    </section>

    <section class="section">
      <div class="container">
        <div class="columns pd is-desktop">
          <div class="column is-1 has-text-centered">
            <i class="fa fa-cog is-primary"></i>
          </div>
          <div class="column is-one-third-desktop">
            <p class="title"><strong>We provide the best games inspiring the world.</strong></p>
          </div>
          <div class="column">
            <p>We are a home based game studio providing the best games on demand. We believe in excelence, we provide fun and we are looking forward to be part of your history.</strong></p>
          </div>
        </div>
      </div>

      <div class="columns pd">
        <div class="column">
          <div class="card">
            <div class="card-content">
              <p class="title">"Awesome!. I can't wait for the next game"</p>
              <p class="subtitle">- Mathew Douglas</p>
            </div>
          </div>
        </div>
        <div class="column">
          <div class="card">
            <div class="card-content">
              <p class="title">"I think it's an absolutely excellent studio. We work together since 2013, now we're a family."</p>
              <p class="subtitle">- Jenny Andrew</p>
            </div>
          </div>
        </div>
        <div class="column">
          <div class="card">
            <div class="card-content">
              <p class="title">"I work here and this is the best game studio, truly the best team. Be here and be forced to agree!."</p>
              <p class="subtitle">- Tony Stark</p>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: 'home',
  data () {
    return {
      heading: 'The power of our imagination make us infinite',
      subheading: 'We have the privilege of working with some of the most brilliant professionals.'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="sass" scoped>
@import '../mq'

.hero
  background: url(https://thecybersafetylady.com.au/wp-content/uploads/2013/11/Screen-Shot-2013-11-24-at-7.38.23-pm.png)
  background-size: cover

  .title
    +mobile
      font-weight: bold
      color: #d8d8d8
    +tablet
      font-size: 2.5rem
      color: #d8d8d8
    +desktop
      font-size: 4rem
      margin-top: 5rem
      color: #d8d8d8

.sub
    +mobile
      color: #d8d8d8
    +tablet
      font-size: 1.5rem
      color: #d8d8d8
    +desktop
      font-size: 1rem
      margin-top: 5rem
      color: #d8d8d8

h2
  margin: 1.5rem 0 2rem 0 !important

.fa-cog
  font-size: 40px

#learn
  +desktop
    margin-bottom: 2rem

.pd
  +tablet
    padding: 2em 0



</style>
