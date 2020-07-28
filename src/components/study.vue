<template>
  <div>
    <template v-if="loginType === 'username'">
      <label>Username</label>
      <input placeholder="Enter your username" key="username-input">
      <button @click="toggleLoginType">Toggle login type</button>
    </template>
    <template v-else>
      <label>Email</label>
      <input placeholder="Enter your email address" key="email-input">
      <button @click="toggleLoginType">Toggle login type</button>
    </template>
  </div>

</template>

<script>
export default {
  data() {
    return {
      loginType: 'username'
    }
  },
  methods: {
    toggleLoginType: function () {
      return this.loginType = this.loginType === 'username' ? 'email' : 'username'
    }
  }
}
</script>