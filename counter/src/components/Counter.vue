<template>
  <div>
   <h1> Counter </h1>
  <h1> {{count}}</h1>
  </div>
  <div>
   <button class="button button1" @click="increaseCount">Increase</button>
   <button class="button button2" @click="decreaseCount">Decrease</button>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data(){
    return{
      count: 0
    }
  },
  props: {
    msg: String
  },
  methods: {
  increaseCount(){
   this.count++
  },
  decreaseCount(){
    this.count--
  }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.button {
  border: none;
  color: white;
  padding: 16px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 10px 10px;
  transition-duration: 0.4s;
  cursor: pointer;
}

.button1 {
  background-color: white;
  color: black;
  border: 2px solid #3ef870;
}

.button1:hover {
  background-color: #1fee56;
  color: white;
}

.button2 {
  background-color: white;
  color: black;
  border: 2px solid #008CBA;
}

.button2:hover {
  background-color: #008CBA;
  color: white;
}


</style>
