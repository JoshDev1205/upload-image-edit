<template>
	<div class="w-full px-10 flex justify-around">
		<Button
			actionType="primary"
			outline
		>
			Cancelar
		</Button>
		<Button actionType="primary">
			Guardar
		</Button>
	</div>
</template>

<script>
import Button from '../Button'
export default {
	name: 'Footer',
	components: {
		Button
	}
}
</script>
