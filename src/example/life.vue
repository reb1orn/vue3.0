<template>
  <div id="life">
    
  </div>
</template>

<script>
// 1. 从 vue 中引入 多个生命周期函数
import {onBeforeMount, onMounted, onBeforeUpdate, onUpdated, onBeforeUnmount} from 'vue'
export default {
  name: "life",
  //setup代替beforeCreate和created两个生命周期函数，执行时间在beforeCreate 和 created 之间
  setup(props,context){
     
    onBeforeMount(() => {
          // 在挂载前执行某些代码
          console.log(1,'挂载前');
      })

      onMounted(() => {
          // 在挂载后执行某些代码
          console.log(2,'挂载后');
      })

      onBeforeUpdate(() => {
          // 在更新前前执行某些代码
          console.log(3,'更新前');
      })

      onUpdated(() => {
          // 在更新后执行某些代码
          console.log(4,'更新后');
      })

      onBeforeUnmount(() => {
          // 在组件销毁前执行某些代码
          console.log(5,'销毁前');
      })

    //   unMounted(() => {
    //       // 在组件销毁后执行某些代码
    //       console.log(6,'销毁后');
    //   })


    return {}
  }
};
</script>
