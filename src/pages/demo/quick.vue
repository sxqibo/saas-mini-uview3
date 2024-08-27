<template>
	<view>
		<up-picker :show="show" :columns="columns"></up-picker>
		<up-button @click="show = true">打开</up-button>
	</view>
</template>

<script setup>
import { ref, reactive } from 'vue';

const show = ref(false);
const columns = reactive([
  ['中国', '美国', '日本']
]);
</script>