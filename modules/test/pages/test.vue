<template>
  <div>
    <el-card class="box-card">
      <el-row class="mb-4">
        <NuxtLink to="/" class="link-base">
          <el-button type="success">Homepage</el-button>
        </NuxtLink>
      </el-row>
      <el-card shadow="never">
        <p style="text-align: center">
          Current route: <code>{{ route.path }}</code>
        </p>
      </el-card>
    </el-card>
    <h1 style="text-align: center">Test page added by module</h1>
    <el-calendar v-model="value" />
  </div>
</template>
<script setup lang="ts">
const route = useRoute();
import { ref } from "vue";
const value = ref(new Date());
</script>
<style>
.link-base {
  text-decoration: auto;
}
</style>
