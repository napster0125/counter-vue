<template>
	<Timer msg="Welcome to Your Vue.js + TypeScript App"/>
</template>

<script lang="ts">
	import { Options, Vue } from 'vue-class-component'
	import Timer from '@/components/Timer.vue' // @ is an alias to /src

	@Options({
		components: {
			Timer
		}
	})
	export default class Home extends Vue {}
</script>

<!-- <style scoped lang="css" src="../styles/common/reset.css"></style> -->
<style lang="scss" scoped>
	@import '../styles/app/common.scss';

</style>
