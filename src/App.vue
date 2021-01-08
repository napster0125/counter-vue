<template>
	<router-view/>
	<template v-if="isDev">
		<link href="tailwind-priority-1.min.css" rel="preload" as="style">
		<link href="tailwind-priority-1.min.css" rel="stylesheet">
	</template>
</template>

<script>
	import {Options, Vue} from "vue-class-component";

	@Options({})
	export default class Timer extends Vue {
		isDev = process.env.NODE_ENV === 'development'
	}
</script>
