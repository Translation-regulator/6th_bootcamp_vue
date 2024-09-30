<script setup>
  import { ref } from 'vue';
  import Header from './Header.vue';
  import Nav from './Nav.vue';
  import Main from './Main.vue';
    // 定義當前頁面
    let visibleSection = ref('CV');

    // 更新 visibleSection 的方法
    function handleSectionUpdate(section) {
    visibleSection.value = section; // 每次觸發事件後的畫面
}
</script>

<template>
  <Header></Header>
  <Nav @updateSection="handleSectionUpdate" />
  <div class="content">
    <Main :visibleSection="visibleSection" /> 
  </div>
</template>

<style scoped>
  .content{
      display: flex;justify-content: center;
      min-height: 100vh;
  }

</style>
