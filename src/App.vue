<template>
  <div id="app">
    <div class="nav has-shadow">
      <div class="container">
        <div class="nav-left">
          <a class="nav-item">Spitzer Game Studio</a>
        </div>

        <span class="nav-toggle" v-on:click="toggleNav" v-bind:class="{ 'is-active': isActive }">
          <span></span>
          <span></span>
          <span></span>
        </span>

        <div class="nav-right nav-menu" v-bind:class="{ 'is-active': isActive }">

          <router-link to="/" class="nav-item r-item">Home</router-link>
          <router-link to="faq" class="nav-item r-item">Features</router-link>
          <router-link to="faq" class="nav-item r-item">About</router-link>
          <router-link to="faq" class="nav-item r-item">Testimonials</router-link>

          <div class="nav-item">
            <p class="control">
              <a class="button is-primary is-outlined">
                <span class="icon">
                  <i class="fa fa-sign-in"></i>
                </span>
                <span>Sign in</span>
              </a>
            </p>
          </div>

        </div>
      </div>
    </div>

    <router-view></router-view>

    <footer class="footer is-primary">
      <div class="container">
        <div class="columns">
          <div class="column">
            <p>Apply now and tell us what kind of game you want.</p>
          </div>
          <div class="column has-text-right">
            <a class="icon" href="#"><i class="fa fa-facebook"></i></a>
            <a class="icon" href="#"><i class="fa fa-twitter"></i></a>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'app',
  data: function() {
    return {
      isActive: false
    }
  },
  methods: {
    toggleNav: function() {
      this.isActive = !this.isActive;
    }
  }
}
</script>

<style lang="sass">
@import "../node_modules/bulma/sass/utilities/initial-variables"
$link-hover: white

@import '../node_modules/bulma/bulma.sass'
@import 'mq'



.nav
  background-color: #383838
  a:hover 
  color: white

.nav-left a 
  color: #fff
  font-weight: bold

.custom-nav-item
 a:hover 
  color: white

.nav-toggle span
  background-color: white

footer
  background-color: $primary !important
  color: #fff

  .icon
    color: #fff
    margin-left: 20px

</style>
