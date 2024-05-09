<script setup>
import { ref } from 'vue'
import { useData } from 'vitepress'
import { ElButton, ElMessage, ElCalendar, ElBacktop } from 'element-plus'

const { page } = useData()

const count = ref(0)
const value = ref(new Date())

const open = () => {
  ElMessage.success('this is a message.')
}
</script>

<template>
  <p>The count is: {{ count }}</p>
  <p>The page is: {{ page }}</p>
  <div class="contaniner">
    <button class="button" @click="count++">Increment</button>
  </div>
  <!-- 使用elementPlus组件 -->
  <el-button type="primary" @click="open" style="margin-bottom: 15px;">我是 ElButton</el-button>
  <!-- 展示图片 -->
  <p>❤️杨紫❤️</p>
  <img src="https://image.baidu.com/search/down?url=https://wx4.sinaimg.cn/large/006ufPaEly1ho9agdfjvvj31l32dm4qq.jpg" />
  <el-calendar v-model="value" />
  <el-backtop />
</template>

<style lang="less">
.contaniner {
  margin-bottom: 20px;
  .button {
    color: red !important;
    font-weight: bold;
  }
}
</style>