<template>
  <div id="reactive">
      {{state.value}}
     {{state.a}}
  </div>
</template>

<script>
// 引入reactive函数
// 创建一个响应式的数据对象
// 该API也很好地解决了Vue2通过defineProperty 实现数据响应式的缺陷
import {reactive} from 'vue'
export default {
  name: "reactive",
  setup(props,context){

    const state = reactive({value:'reactive函数',a:2})

    return {state}
  }
};
</script>
