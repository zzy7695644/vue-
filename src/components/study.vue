<template>
  <!-- <div v-bind:style="{ color: activeColor, fontSize: fontSize+'px'}"></div> -->
  <!-- <div v-bind:style="styleObject">1111111111111111111111111111111111</div> -->
  <!-- 直接绑定样式对象，return里应该是样式名加参数 -->
  <!-- <div v-bind:style="[baseStyles, overridingStyles]">111111111111111111111111</div> -->
  <!-- 绑定多个样式对象 -->
  <div :style="{ display: ['-webkit-box', '-ms-flexbox', 'flex'] }">22222222222222222</div>
</template>

<script>
export default {
  data() {
    return {
      baseStyles: {
        color: 'red'
      },
      overridingStyles:{
        fontSize: 30
      }
      
    }
  },
  
}
</script>