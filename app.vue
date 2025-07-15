<template>
  <div>
    <Paginator :rows="10" :totalRecords="100" :pageLinkSize="5">
      <template #container="data">
        <div style="gap: 20px; display: flex; flex-direction: column">
          <div>{{ data }}</div>
          <div>{{ data.pageLinks?.[0] }}</div>
        </div>
      </template>
    </Paginator>
  </div>
</template>
<script setup lang="ts"></script>
