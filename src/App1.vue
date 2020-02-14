<template>
  <div>
    <h2>app根组件</h2>
    <p>{{city}}</p>
    <p>
      <input type="text" v-model="city" />
    </p>

    <p>
      <input type="text" :value="city" @input="city=$event.target.value" />
    </p>
  </div>
</template>

<script>
export default {
  name: 'app1',
  data() {
    return {
      city: '北京'
    }
  }
}
</script>

<style lang="less" scoped>
</style>
