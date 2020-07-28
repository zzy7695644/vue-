<template>
  <!-- <div v-bind:class="[activeClass, errorClass]"></div> -->
  <!-- <div v-bind:class="[isActive ? activeClass : '', errorClass]"></div> -->
  <!-- isActive不为truthy真值（除 false、0、""、null、undefined 和 NaN 以外皆为真值） -->
  <div v-bind:class="[{ active: activeClass }, errorClass]"></div>
  <!-- 对象里的值是由data里数据的真假值决定 -->
  <!-- 疑问：class属性只取key值 -->
</template>

<script>
export default {
  data() {
    return {
       activeClass: true,
       errorClass: 'text-danger'
    }
  }
}
</script>