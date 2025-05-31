<template>
  <div id="mainlayout">
    <el-container>
      <el-aside class="layer-side">
        <GlobalSide />
      </el-aside>
      <el-container class="layer-container">
        <el-main>
          <RouterView />
        </el-main>
      </el-container>
    </el-container>
  </div>
</template>

<script setup lang="ts">
import GlobalSide from "@/components/GlobalSide.vue";
</script>

<style scoped>
/* #mainlayout .footer {
  background: #ececec;
  text-align: center;
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  padding: 16px;
}
.el-header {
  --el-header-padding: 0 0px;
} */
#mainlayout .layer-side {
  width: 200px;
}
#mainlayout .layer-header {
  background: #fff;
}
#mainlayout .layer-container {
  margin-left: auto;
}
</style>
