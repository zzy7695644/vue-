<template>
  <div>
    <button v-on:click="say('hi')">say hi</button>
    <button v-on:click="say('what')">say what</button>
    <button v-on:click="warn('Form cannot be submitted yet.',$event)">Submit</button>
    <input v-on:keyup.alt.67="clear">
  </div>
</template>

<script>
export default {
  data() {
    return{
      name: 'vue.js'
    }
  },
  methods: {
    say: function(message){
      alert(message)
    },
    warn: function(message, event){
      console.log(event)
      if(event){
        event.preventDefault()
        console.log(event.preventDefault())
      }
      alert(message)
    }
    
  }
}
</script>
