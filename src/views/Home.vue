<template>
  <div class="home">
    <!-- template中使用环境变量 -->
    API: {{ api }}
  </div>
</template>

<script>
export default {
  name: 'home',
  data() {
    return {
      api: process.env.VUE_APP_API,
    };
  },
  mounted() {
    // js代码中使用环境变量
    console.log('BASE_URL: ', process.env.BASE_URL);
    console.log('VUE_APP_API: ', process.env.VUE_APP_API);
  },
};
</script>
