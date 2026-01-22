<template>
  <div class="feature-view">
    <PageTitle msg="特色功能" />
    <h1>特色功能页面</h1>
    <p>展示 Hollow Knight 项目的各种特色功能</p>
    
    <!-- 地图画廊组件 -->
    <div style="margin: 30px 0;">
      <MapBackgroundGallery />
    </div>
    
    <!-- 其他功能展示 -->
    <div class="other-features">
      <h3>🚀 其他特色功能</h3>
      <div class="feature-grid">
        <div class="feature-card">
          <h4>地图系统</h4>
          <p>交互式地图探索</p>
        </div>
        <div class="feature-card">
          <h4>故事模式</h4>
          <p>沉浸式剧情体验</p>
        </div>
        <div class="feature-card">
          <h4>画廊展示</h4>
          <p>艺术概念图集</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import PageTitle from '@/components/PageTitle.vue'
import MapBackgroundGallery from '@/components/gallery/MapBackgroundGallery.vue'
</script>

<style scoped>
.feature-view {
  padding: 20px;
  color: #f0e6d2;
  max-width: 1200px;
  margin: 0 auto;
}

h1 {
  color: #4ecdc4;
  margin: 20px 0 10px 0;
}

.other-features {
  margin-top: 40px;
  padding: 25px;
  background: rgba(40, 35, 30, 0.7);
  border-radius: 12px;
  border: 1px solid #5d4d3a;
}

.feature-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 20px;
  margin-top: 20px;
}

.feature-card {
  padding: 20px;
  background: rgba(255, 255, 255, 0.05);
  border-radius: 8px;
  border: 1px solid rgba(255, 255, 255, 0.1);
  transition: transform 0.3s;
}

.feature-card:hover {
  transform: translateY(-5px);
  background: rgba(255, 255, 255, 0.1);
}

.feature-card h4 {
  color: #e8d8b8;
  margin-bottom: 10px;
}
</style>
