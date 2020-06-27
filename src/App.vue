<template>
  <div id="app">
    <GgHeader />
    <router-view />
  </div>
</template>

<script>
import GgHeader from "@/components/GgHeader.vue";

export default {
  components: {
    GgHeader
  }
};
</script>
