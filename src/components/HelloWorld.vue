<script setup>
import { ref } from 'vue'
import { ElButton } from 'element-plus';

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template>
  <h1 class="header">{{ msg }}</h1>

  <div class="card">
    <el-button type="button" @click="count++">count is {{ count }}</el-button>
    <p>
      Edit
      <code>components/HelloWorld.vue</code> to test HMR
    </p>
  </div>

  <p>
    Check out
    <a href="https://vuejs.org/guide/quick-start.html#local" target="_blank"
      >create-vue</a
    >, the official Vue + Vite starter
  </p>
  <p>
    Learn more about IDE Support for Vue in the
    <a
      href="https://vuejs.org/guide/scaling-up/tooling.html#ide-support"
      target="_blank"
      >Vue Docs Scaling up Guide</a
    >.
  </p>
  <p class="read-the-docs">Click on the Vite and Vue logos to learn more</p>
</template>

<style scoped>
.header {
  position: relative;
}
.header::before,
.header::after {
  bottom: 0;
  content: '';
  position: absolute;
  top: 0;
  width: 10px;
}
.header::before {
  background-color: #9773f7;
  left: 0;
}
.header::after {
  background-color: #64b687;
  right: 0;
}
.read-the-docs {
  color: #888;
}
</style>
