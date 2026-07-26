<template>
  <div class="glass-card ticker-card">
    <div class="ticker-wrapper">
      <div v-for="(item, index) in tickerItems" :key="index" class="ticker-item">
        <span>{{ item.text }}</span>
        <span style="color: var(--success-color); font-weight: bold;">[生成完成]</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const tickerItems = ref([
  {
    "text": "用户 138****7721 完成了国潮新茶饮与非遗文化联名脑暴方案"
  },
  {
    "text": "用户 189****4409 生成了小红书爆款科普短视频 5 个颠覆性选题"
  },
  {
    "text": "用户 131****8820 完成了智能手表发布会沉浸式互动体验设计"
  },
  {
    "text": "用户 153****1192 生成了社区咖啡店周年庆线下打卡玩法"
  },
  {
    "text": "用户 177****6639 获得了独立独立游戏悬疑剧情反转灵感"
  }
]);
</script>
