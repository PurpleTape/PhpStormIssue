<template>
  <MyComponent1/>
  <MyComponent1NoIDEError/>
  <MyComponent2/>
</template>

<script setup lang="ts">
import MyComponent1 from '@components/MyComponent1.vue';
import MyComponent2 from '@components/MyComponent2.vue';
import MyComponent1NoIDEError from '#components/MyComponent1.vue';
</script>
