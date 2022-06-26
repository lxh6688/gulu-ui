<template>
  <div class="cascaderItem">
    {{ sourceItem.name }}
    <div v-if="sourceItem.children">
      <gulu-cascader-item
        v-for="item in sourceItem.children"
        :key="item.name"
        :sourceItem="item"
      ></gulu-cascader-item>
    </div>
  </div>
</template>

<script>
export default {
  name: "GuluCascaderItem",
  props: {
    sourceItem: {
      type: Object,
    },
  },
};
</script>

<style scoped lang="scss">
.cascaderItem {
  border: 1px solid red;
  margin: 10px;
}
</style> 