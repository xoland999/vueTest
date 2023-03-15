<template>
  <div :style="{ display: 'flex' }">
    <a-card class="card-demo" title="Custom hover style" hoverable>
      <template #cover>
        <div>
          <img src="" />
        </div>
      </template>
      <template #extra>
        <!-- <a-link>More</a-link> -->
      </template>
      <a-descriptions :data="data" :column="1" title="User Info" bordered />
    </a-card>
  </div>
</template>
<script lang="ts">
import { defineComponent } from "vue";
export default defineComponent({
  name: "BookFront",
  setup() {
    const data = [
      {
        label: "名稱",
        value: "aaa",
      },
      {
        label: "作者",
        value: "bbb",
      },
      {
        label: "描述",
        value: "ccccccccccccccccccccccccccccccccccccccccccccc",
      },
    ];
    return { data };
  },
});
</script>
<style scoped>
.card-demo {
  width: 360px;
  margin-left: 24px;
  transition-property: all;
}
.card-demo:hover {
  transform: translateY(-4px);
}
</style>
