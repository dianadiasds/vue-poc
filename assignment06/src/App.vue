<template>
  <div class="container" id="app">
    <app-header></app-header>
    <hr>
    <div class="row">

        <app-list></app-list>


        <app-update></app-update>

    </div>
    <hr>
    <div class="row">

        <app-footer></app-footer>

    </div>
  </div>
</template>

<script>
  import Header from "./components/Header"
  import List from "./components/List"
  import Update from "./components/Update"
  import Footer from "./components/Footer"

  export default {

    components: {
      'app-header' : Header,
      'app-list' : List ,
      'app-update' : Update,
      'app-footer' : Footer
    },
  }
</script>

<style>

</style>
