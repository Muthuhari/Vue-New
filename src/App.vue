<!--
  Composition API (new)
  <script setup>
import {ref} from "vue"

let count = ref(0)
</script>

<template>
<main>
      <container class="container">
        <h4>the current count is...</h4>
        <h1>{{count}}</h1>
        <button @click="count++">+</button>
        <button @click="count--">-</button>
      </container>
  </main>
</template>

<style scoped>
main {
  width: 100vw;
  height: 100vh;
  background-color: aliceblue;
  display: flex;
  align-items: center;
  justify-content: center;
}

.container {
  text-align: center;
}
</style>-->


<template>
<main>
      <container class="container">
        <h2>The current count is..</h2>
        <h1>{{count}}</h1>
        <button @click="addToCount()">+</button>
        <button @click="subtractFromCount()">-</button>
      </container>
  </main>
</template>
{/*Option API (Odl, but use in company- here use export default.........) */}
<script >
export default({
  data(){
    return{
      count: 0
    }
  },
  methods: {
    addToCount(){
      this.count = this.count +1
    },
    subtractFromCount(){
      this.count = this.count -1
    }
  }
})
</script>

<style scoped>
main {
  
  width: 100vw;
  height: 100vh;
  background-color: aliceblue;
  display: flex;
  align-items: center;
  justify-content: center;
}

.container {
  text-align: center;
}
button {
  font-size: 6em;
  background-color: blue;
  color: white;
}
h2{
  font-size: 3em;
} 
h1{
  font-size: 5em;
  color: green;
} 
</style>