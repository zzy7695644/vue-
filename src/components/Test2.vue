<template>
  <div>
    <input type="checkbox" id="jack" value="Jack" v-model="checkedNames">
    <label for="jack">Jack</label>
    <input type="checkbox" id="john" value="John" v-model="checkedNames">
    <label for="john">John</label>
    <input type="checkbox" id="mike" value="Mike" v-model="checkedNames">
    <label for="mike">Mike</label>
    <br>
    <span>Checked names: {{ checkedNames }}</span>
    <!-- 多个复选框绑定到同一个数组 -->
  </div>
</template>

<script>
export default {
  data() {
    return{
      checkedNames: ['ssss']
    }
  }
}
</script>