<template>
  <div class="static" v-bind:class= "{active: isActive, 'text-danger': hasError}">
    
  </div>
</template>

<script>
export default {
  data() {
    return {
       isActive: true,
       hasError: true
    }
  }
}
</script>