<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <br>
    <button class="btn btn-primary" @click="gotoDaybook">primary</button>
    <button class="btn btn-secondary">secondary</button>
    <button class="btn btn-success">Success</button>
  </div>
</template>

<script>
export default {
  methods:{
    gotoDaybook(){
      this.$router.push(({name:'no-entry'}))
    }
  }
}
</script>
