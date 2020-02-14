<template>
  <div>
    <h2>app根组件</h2>
    <p>当前父组件的city {{city}}</p>
    <!-- <comp-input :value="city" @input="(data)=>{city=data}"></comp-input> -->
    <!-- <com-input :value="city" @input="abc"></com-input> -->
    <com-input v-model="city"></com-input>
  </div>
</template>

<script>
import ComInput from './components/ComInput.vue'
export default {
  name: 'App',
  components: {
    ComInput
  },
  data() {
    return {
      city: 'tom'
    }
  }
}
</script>

<style lang="less" scoped>
</style>
