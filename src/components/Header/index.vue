<template>
	<div class="w-full p-4 flex justify-between">
		<Button actionType="icon" iconType="arrow" />
		<Button actionType="icon" />
	</div>
</template>

<script>
import Button from '../Button'
export default {
	name: 'Header',
	components: {
		Button
	}
}
</script>

<style lang="scss" scoped>
</style>
