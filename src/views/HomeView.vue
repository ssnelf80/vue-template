<script setup lang="ts">
import { AgGridVue } from "ag-grid-vue3";
import "ag-grid-community/dist/styles/ag-grid.css";
import "ag-grid-community/dist/styles/ag-theme-material.css";
import { ref } from "vue";

const columnDefs = ref([
  { headerName: "Make", field: "make" },
  { headerName: "Model", field: "model" },
  { headerName: "Price", field: "price" },
]);
const rowData = ref([
  { make: "Toyota", model: "Celica", price: 35000 },
  { make: "Ford", model: "Mondeo", price: 32000 },
  { make: "Porsche", model: "Boxter", price: 72000 },
]);
</script>

<template>
  <div>
    <el-row>
      <el-button type="primary">Primary</el-button>
      <el-button type="success">Success</el-button>
      <el-button type="info">Info</el-button>
    </el-row>
    <ag-grid-vue

      class="table ag-theme-material"
      :columnDefs="columnDefs"
      :rowData="rowData"
    >
    </ag-grid-vue>
  </div>
</template>
<style>
@import "../assets/root.css";
    .table {
      width: calc(100vw - var(--aside-width));
      height: 400px;
    }
</style>

