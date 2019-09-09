<template>
	<button class="h-12 w-12 bg-main-black rounded text-white flex justify-center py-3">
		<component :is="iconTypeValidation" />
	</button>
</template>

<script>
import Arrow from './Arrow'
import Delete from './Delete'
export default {
	components: {
		Arrow,
		Delete
	},
	name: 'IconButton',
	props: ['iconType'],
	computed: {
		iconTypeValidation () {
			return this.iconType === 'arrow' ? Arrow : Delete
		}
	}
}
</script>

<style>
</style>
