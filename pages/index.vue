<template>
  <div>
    <el-card class="box-card">
      <el-row class="mb-4">
        <NuxtLink to="/test" class="link-base">
          <el-button type="success">Test Page</el-button>
        </NuxtLink>
      </el-row>
      <el-card shadow="never">
        <p style="text-align: center">
          Current route: <code>{{ route.path }}</code>
        </p>
      </el-card>
    </el-card>
  </div>
</template>
<script setup lang="ts">
const route = useRoute();
</script>
<style>
.link-base {
  text-decoration: auto;
}
</style>
