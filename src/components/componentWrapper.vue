<template>
  <div :id="title" class="wrapper">
    <h2>{{ title }}</h2>
    <div class="content">
      <slot><p class="tips">暂无示例，待补充</p></slot>
    </div>
  </div>
</template>

<script setup>
const props = defineProps({
  title: {
    type: String,
    default: 'component name'
  }
})
</script>

<style lang="scss" scoped>
.wrapper {
  margin-bottom: 24px;
  padding: 12px 0;
  border-bottom: 2px dashed #eee;
}

h2 {
  height: 32px;
  font-weight: bold;
  display: flex;
  align-items: center;
  &::before {
    content: "⭕️";
    font-size: 16px;
    margin-right: 8px;
  }
}

.content {
  margin-top: 12px;
  padding: 12px;
  border: 1px solid #ccc;
}

.tips {
  color: #999;
}
</style>
