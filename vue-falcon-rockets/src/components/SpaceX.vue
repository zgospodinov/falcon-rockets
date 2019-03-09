<template>
  <div class="space">
  
    <h1>Space X</h1>
    <h3>{{msg}}</h3>
  </div>
</template>

<script>
  export default {
    name: 'SpaceX',
    props: {
      msg: String
    },
    methods: {
      obtainRockets() {
        let url = "https://api.spacexdata.com/v2/rockets";
        fetch(url).then(response => console.log(response.json()));
      }
    },
    data() {
      return {
  
      }
    },
    created() {
      this.obtainRockets();
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  
</style>
