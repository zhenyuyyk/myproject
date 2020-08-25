<template>
  <div class="home">
    jenkins测试项目<br></br>
    我在 {{ process.NODE_ENV }} 环境，url为：{{ process.VUE_APP_URL }}
  </div>
</template>

<script>

export default {
  name: 'Home',
  data() {
    return {
      process:process.env
    }
  },
  created() {
    console.log(process.env)
  },
  methods: {}
}
</script>
