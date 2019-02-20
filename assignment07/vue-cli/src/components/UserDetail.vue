<template>
    <div class="component">
        <h3>You may view the User Details here</h3>
        <p>Many Details</p>
        <p>My name: {{ switchName() }}</p>
        <button @click="resetName">reset name</button>
    </div>
</template>

<script>
  export default {
    props: {
      myName: {
        type: String,
        require: true
      }
    },
    methods: {
       switchName (){
        return this.myName.split("").reverse().join("")
      },
      resetName () {
         this.myName = "Diana";
         this.$emit('nameWasReset', this.myName)
      }
    }
  }
</script>

<style scoped>
    div {
        background-color: lightcoral;
    }
</style>
