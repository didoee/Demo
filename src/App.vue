<script setup>
import { ref } from 'vue';
const value1 = ref('');

const hanleChange = (value) => {
	console.log(value);
	value1.value = value;
};
</script>

<template>
	<el-date-picker
		:value="value1"
		@change="hanleChange"
		type="daterange"
		range-separator="To"
		start-placeholder="Start date"
		end-placeholder="End date"
	/>
</template>
