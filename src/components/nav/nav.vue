<script setup lang="ts">
import myBtn from "@/components/button/index.vue";
import { ref } from "vue";
let hi = ref(false);
</script>

<template>
  <nav>
    <router-link to="/"
      ><my-btn round icon="icon-shouye">首页</my-btn></router-link
    >
    <my-btn round @click="hi = !hi">基础组件</my-btn>
    <div v-show="hi">
      <router-link to="/button"
        ><my-btn round icon="icon-anniu">按钮</my-btn></router-link
      >
      <router-link to="/input"
        ><my-btn round icon="icon-B-shurukuang">输入框</my-btn></router-link
      >

      <router-link to="/switch"
        ><my-btn round icon="icon-gongyezujian-kaiguan"
          >开关</my-btn
        ></router-link
      >
      <router-link to="/table"
        ><my-btn round icon="icon-gongyezujian-kaiguan"
          >表格</my-btn
        ></router-link
      >
      <router-link to="/divider"
        ><my-btn round icon="icon-gongyezujian-kaiguan"
          >分割线</my-btn
        ></router-link
      >
    </div>
    <router-link to="/card"> <my-btn round>卡片</my-btn></router-link>
    <router-link to="/dialog"> <my-btn round>对话框</my-btn></router-link>
    <router-link to="/message"> <my-btn round>消息</my-btn></router-link>
    <router-link to="/toolTip"> <my-btn round>提示框</my-btn></router-link>
    <router-link to="/smoke"> <my-btn round>烟雾</my-btn></router-link>
    <router-link to="/sweepstake"> <my-btn round>抽奖</my-btn></router-link>
  </nav>
</template>

<style scoped>
a {
  text-decoration: none;
  color: inherit;
  margin-left: 3px;
}
nav {
  position: fixed;
  right: 10px;
  top: 10px;
  display: flex;
  flex-direction: column;
}
button {
  width: 6rem;
}
</style>
