<template>
  <h1>{{ msg }}</h1>

  <div class="card">
    <button type="button" @click="count++">count is {{ count }}</button>
    <p>
      Edit
      <code>components/HelloWorld.vue</code> to test HMR
    </p>
  </div>

  <p>
    Check out
    <a href="https://vuejs.org/guide/quick-start.html#local" target="_blank"
      >create-vue</a
    >, the official Vue + Vite starter
  </p>
  <p>
    Install
    <a href="https://github.com/vuejs/language-tools" target="_blank">Volar</a>
    in your IDE for a better DX
  </p>
  <p class="read-the-docs">Click on the Vite and Vue logos to learn more</p>
</template>

<script>// dont do this for options api: <script setup>
//this is composition api
/* import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0) */

//this is options api below
export default{ //import {ref} from 'vue'
//props is used to pass data from parent to child   , emitter passes from child to parent
  props:['msg'],//this is the props option which is an array containing names of props we are defining
  //all options have a comma after
  //data option- is going to contain variables
  data(){//this is the data option ,it is a function of sorts
    return{//we are returning the variables we will use
      count:0,//this is a variable initialised to 0
    }
  },
};


</script>


<style scoped>/* scoped means it will only apply to this component*/
.read-the-docs {
  color: #888;
}
</style>
