<template>
  <div class="login-page">
    <div class="login-box">
      <h2 class="login-title">Welcome</h2>
      <input type="text" v-model="username" placeholder="用户名"/>
      <input type="password" v-model="password" placeholder="密码"/>
      <button @click="handleClick">登录</button>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      username: '',
      password: ''
    }
  },
  methods: {
    handleClick () {
      // 处理登录
    }
  }
}
</script>

<style>
.login-page {
  text-align: center;
}

.login-box {
  display: inline-block;
  padding: 15px;
  width: 300px;
  background: #fff;
  border-radius: 10px;
  box-shadow: 0 0 8px #ccc;
}

.login-title {
  font-size: 20px;
  font-weight: bold;
  margin-bottom: 15px;
}

input {
  display: block;
  width: 100%;
  padding: 8px 10px;
  border: 1px solid #ccc;
  outline: none;
  margin-bottom: 10px;
  font-size: 14px;
  color: #555;
}

button {
  display: block;
  width: 100%;
  padding: 8px 10px;
  background: #00bcd4;
  border: none;
  outline: none;
  font-weight: bold;
  font-size: 16px;
  color: #fff;
  border-radius: 4px;
  cursor: pointer;
}
</style>
