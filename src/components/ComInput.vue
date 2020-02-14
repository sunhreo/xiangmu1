<template>
  <div>
    <!-- 如下输入框value发生变化 父组件要感知到 @input事件:可以感知内容发生变化-->
    用户名:
    <input type="text" :value="value" @input="$emit('input',$event.target.value)" />
  </div>
</template>

<script>
export default {
  name: 'com-input',
  props: ['value']
}
</script>

<style lang="less" scoped>
</style>
