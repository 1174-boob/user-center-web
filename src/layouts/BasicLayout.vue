<template>
  <div id="basicLayout">
    <a-layout>
      <a-layout-header class="header">
        <GlobalHeader />
      </a-layout-header>
      <a-layout-content class="content">
        <router-view />
      </a-layout-content>
      <a-layout-footer class="footer"
        ><a href="https://baidu.com" target="_blank">去百度啦</a></a-layout-footer
      >
    </a-layout>
  </div>
</template>

<script lang="ts" setup>
  import GlobalHeader from '@/components/GlobalHeader.vue'
</script>

<style scoped>
  #basicLayout .footer {
    background: gray;
    text-align: center;
    position: fixed;
    bottom: 0;
    right: 0;
    left: 0;
    padding: 16px;
  }

  #basicLayout .content {
    padding: 20px;
    margin-bottom: 20px;
    background: linear-gradient(to right, #fefefe, #fff);
  }

  #basicLayout .header {
    background: white;
    margin-bottom: 16px;
    color: unset;
    padding-inline: 20px;
  }
</style>
