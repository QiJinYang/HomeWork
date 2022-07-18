<template>
  <div class="home">
    <qjyButton>默认按钮</qjyButton>
    <qjyButton type="primary">成功按钮</qjyButton>
    <qjyButton type="danger">危险按钮</qjyButton>
    <qjyButton type="warning">警告按钮</qjyButton>
  </div>
</template>

<script>
export default {
  name: 'Home',
  components: {
    qjyButton: () => import('../components/button/index.vue')
  },
  methods: {
    handleSubmit() {
      this.flag = true
      setTimeout(() => {
        console.log('123')
        this.flag = false
      }, 3000)
    }
  }
}
</script>
