<template>
  <div>
    <p v-for="car in 4" v-bind:key="car" ref="car"> I am car number {{car}}</p>
    <button @click="submit">View refs</button>
  </div>
</template>

<script>
export default {
  name: 'Test',
  data(){
    return {
    }
  },
  methods: {
    submit(){
      console.log(this.$refs)
    }
  }
}
</script>


<style scoped>
p , input, button{
  font-size: 20px;
}
input, button{
  font-size: 20px;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
