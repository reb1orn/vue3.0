<template>
  <div>
    <h1>setup</h1>
    <div id="counter">
        <p>{{number}}</p>
        <button @click="add">增加</button>
    </div>
  </div>
</template>

<script>
// 引入ref函数
import {ref} from 'vue'
export default {
  name: "setup",
  setup(props,context){
    console.log(props,context);
    // ref函数包装一个响应式变量number
    let number = ref(0)

    function add() {
      // number是被ref函数包装过了的，其值保存在.value中
      // console.log(number)
      number.value++
    }

    //  将 number 和 add 返回出去，供template中使用
    return {number,add}
  }
};
</script>
