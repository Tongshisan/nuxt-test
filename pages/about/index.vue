<script setup lang="ts">
import { ref } from 'vue';

console.log('useFetch', useFetch);
const { data: users, error } = await useFetch(
	'https://jsonplaceholder.typicode.com/users'
);
console.log('users', users.value);
</script>

<template>
	<div class="home">
		<h1>About</h1>
	</div>
</template>
