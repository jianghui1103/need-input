<template>
  <div class="zfb-pay">
    <input v-model="password" />
  </div>
</template>

<script>
export default {
  data() {
    return {
      password: "", // 支付密码
    };
  },
  watch: {
    // 监听支付密码，支付密码输入完成后触发input-end回调
    // 通知父组件的同时会把输入完成的密码作为参数告知父组件，即input-end函数的参数能拿到密码
    password(n, o) {
      console.log(n);
    },
  },
  methods: {},
};
</script>
