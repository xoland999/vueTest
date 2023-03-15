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
      <a-space direction="vertical" size="large">
        <a-input
          :style="{ width: '320px' }"
          placeholder="Please enter something"
          allow-clear
        >
          <template #prepend> 名稱 </template>
        </a-input>
        <a-input
          :style="{ width: '320px' }"
          placeholder="Please enter something"
          allow-clear
        >
          <template #prepend> 作者 </template>
        </a-input>
      </a-space>
      <!-- <div>備註</div> -->
    </a-card>
  </div>
</template>
<script lang="ts">
import { defineComponent } from "vue";
export default defineComponent({
  name: "BookFront",
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
