<template>
  <div class="home">
    {{count}}
  </div>
</template>

<script lang="ts">
/**
 * Composition API 用户层面
 * vue 框架
 * hook -> 组合起来 -> Vue3.0 Composition API 框架设计模式
 * */
import { defineComponent, ref } from 'vue'

export default defineComponent({
  name: 'Home',
  setup () {
    console.log('setup')
    const count = ref(0)

    console.log('count==>', count)

    return {
      count
    }
  }
})
</script>
