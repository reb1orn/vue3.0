<template>
  <div>
    <h1>ref</h1>
    <div id="counter">
       
    </div>
  </div>
</template>

<script>
// 引入ref,reactive函数
import {ref,reactive} from 'vue'
export default {
  name: "ref",
  setup(props,context){
    const obj = {count: 3}
      const state1 = ref(obj)
      const state2 = reactive(obj)

      console.log(state1)
      console.log(state2)
  }
};
</script>
