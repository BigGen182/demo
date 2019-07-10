
<template>
  <h3>我是子组件！</h3>
</template>
<script>
  export default {
    mounted: function () {
      this.$emit('getMessage', '我是来自子组件的消息')
    }
  }
</script>
