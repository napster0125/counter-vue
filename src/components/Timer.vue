<template>
	<div class="hello">
		sdf
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

<style lang="scss" scoped>
	@import '../styles/app/common.scss';

	div {
		background-color: rgba(0, 0, 255, 0.1);
	}
</style>
