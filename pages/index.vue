<template>
  <section class="container">
    <div>
    <!-- <Logo /> -->
    <!-- <img class="logo" src="~/assets/img/logo.png" alt="logo"> -->
      <h1 class="title">
        Grocery Store Database
      </h1>
      <div class="links">
        <nuxt-link class="button--grey link" style="margin-left: 15px;" to="/products">View Products</nuxt-link>
        <nuxt-link class="button--grey link" style="margin-left: 15px;" to="/aisles">View Aisles</nuxt-link>
        <nuxt-link class="button--grey link" style="margin-left: 15px;" to="/departments">View Departments</nuxt-link>
        <nuxt-link class="button--grey link" style="margin-left: 15px;" to="/employees">View Employees</nuxt-link>
        <nuxt-link class="button--grey link" style="margin-left: 15px;" to="/customers">View Customers</nuxt-link>
        <nuxt-link class="button--grey link" style="margin-left: 15px;" to="/suppliers">View Suppliers</nuxt-link>
        
      </div>
    </div>
  </section>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style lang="stylus" scoped>
.container
  min-height 90vh
  display flex
  justify-content center
  align-items center
  text-align center

@media (min-height 1080px)
  .container
    margin-top -200px

.title
  font-family "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif /* 1 */
  display block
  font-weight 300
  font-size 100px
  color #35495e
  letter-spacing 1px

.subtitle
  font-weight 300
  font-size 42px
  color #526488
  word-spacing 5px
  padding-bottom 15px

.links
  padding-top 15px
  .link
    display relative
    width 50%
    margin-bottom 10px

@media (max-width 860px)
  .title
    font-size 64px
  .subtitle
    font-size 32px

@media (max-width 860px)
  .links
    .link
      width 50%
      margin-bottom 15px
      display relative

.logo
  display inline-block
  vertical-align middle
</style>
