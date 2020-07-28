<template>
  <ul>
    <li v-for="(item, index) in items" :key="item.message">
      <!-- 一定要绑定:key="item.message"，没绑定提示问题 -->
      {{ parentMessage }} - {{ index }} - {{ item.message }}
    </li>
  </ul>
</template>
<script>
export default {
  data() {
    return {
      parentMessage: 'green',
      items: [{message: 'foo'},
              {message: 'too'}]
    }
  }
}
</script>