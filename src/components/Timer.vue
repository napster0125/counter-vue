<template>
	<div>
		<button class="x bg-gray-400">Button Child</button>
	</div>
</template>

<script lang="ts">
	import { Options, Vue } from 'vue-class-component'

	@Options({
		props: {
			msg: String
		}
	})
	export default class Timer extends Vue {
		msg!: string
	}
</script>

<style scoped lang="scss" src="../styles/app/common.scss"></style>
<style scoped lang="scss">
	button {
		color: yellow;
	}
</style>
