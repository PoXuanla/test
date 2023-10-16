<template>
  <div>
    <div style="display: flex; align-items: center; gap: 10px">
      <img
        style="border-radius: 50%; width: 15px; height: 15px"
        src="./assets/logo.svg"
      />
      <div>梁實秋</div>
      <div>2022/12/05</div>
    </div>
    <!-- 文章內容 -->
    <p>文案內容</p>
    <!-- 圖片 -->
    <div style="display: flex; gap: 15px">
      <div
        style="width: 50px; height: 50px; border: 1px solid black; flex: 1"
      ></div>
      <div
        style="width: 50px; height: 50px; border: 1px solid black; flex: 1"
      ></div>
      <div
        style="width: 50px; height: 50px; border: 1px solid black; flex: 1"
      ></div>
    </div>
  </div>
  <!-- 標籤與其他 -->
  <div>
    <div style="display: flex; gap: 10px; flex-wrap: wrap">
      <p>標籤一</p>
      <!-- <p>標籤二</p>
        <p>標籤二</p> <p>標籤二</p> <p>標籤二</p> <p>標籤二</p> <p>標籤二</p> <p>標籤二</p> <p>標籤二</p> <p>標籤二</p> -->
      <div>點贊收藏評論</div>
    </div>
  </div>
</template>

<script setup>
const props = defineProps({
  post: Object,
});
</script>
