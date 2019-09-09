<template>
	<IconButton
		v-if="actionType === 'icon'"
		:iconType="iconType"
	/>
	<PrimaryButton
		v-bind:outline="outline"
		v-else-if="actionType === 'primary'"
	>
		<slot />
	</PrimaryButton>
</template>

<script>
import IconButton from './IconButton'
import PrimaryButton from './PrimaryButton'
export default {
	name: 'Button',
	components: {
		IconButton,
		PrimaryButton
	},
	props: {
		outline: {
			type: Boolean,
			default: false
		},
		actionType: {
			required: true,
			default: 'primary',
			type: String
		},
		iconType: {
			type: String
		}
	}
}
</script>

<style scoped>
</style>
