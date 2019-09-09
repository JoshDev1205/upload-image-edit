<template>
	<button
		class="tracking-wide shadow-md font-medium leading-none h-10 w-40 rounded-sm "
		:class="this.isOutline"
	>
		<slot />
	</button>
</template>

<script>
export default {
	name: 'PrimaryButton',
	props: ['outline'],
	computed: {
		isOutline () {
			return this.outline ? 'border border-main-blue bg-white text-main-blue' : 'bg-main-teal text-white'
		}
	}
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Roboto:400,500&display=swap');
</style>
