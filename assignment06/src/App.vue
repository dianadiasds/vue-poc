<template>
  <div class="container" id="app">
    <Header/>
    <hr>
    <div class="row">
      <div class="col-xs-12 col-sm-6">
        <List/>
      </div>
      <div class="col-xs-12 col-sm-6">
       <Update/>
      </div>
    </div>
    <hr>
    <div class="row">
      <div class="col-xs-12">
       <Footer/>
      </div>
    </div>
  </div>
</template>

<script>
  import Header from "./components/Header"
  import List from "./components/List"
  import Update from "./components/Update"
  import Footer from "./components/Footer"

  export default {

    components: { Header, List , Update, Footer},
  }
</script>

<style>

</style>
