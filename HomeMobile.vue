<template>
	<div class="homeMobileDiv">
		<Scroll class="scroll" 
			downPullBackgroundColor="ghostwhite" 
			@upPullEvent="onScrollUpPullEvent" 
			@downPullEvent="onScrollDownPullEvent">
			<h1>dfasdfasdfa</h1>
			<h1>dfasdfasdfa</h1>
			<h1>dfasdfasdfa</h1>
			<h1>dfasdfasdfa</h1>
			<h1>dfasdfasdfa</h1>
			<h1>dfasdfasdfa</h1>
			<h1>dfasdfasdfa</h1>
			<h1>dfasdfasdfa</h1>
			<h1>dfasdfasdfa</h1>
			<h1>dfasdfasdfa</h1>
			<h1>dfasdfasdfa</h1>
			<h1>dfasdfasdfa</h1>
			<h1>dfasdfasdfa</h1>
			<h1>dfasdfasdfa</h1>
			<h1>dfasdfasdfa</h1>
			<h1>dfasdfasdfa</h1>
			<h1>dfasdfasdfa</h1>
			<h1>dfasdfasdfa</h1>
			<h1>dfasdfasdfa</h1>
			<h1>dfasdfasdfa</h1>
			<h1>dfasdfasdfa</h1>
			<h1>dfasdfasdfa</h1>
			<h1>dfasdfasdfa</h1>
			<h1>dfasdfasdfa</h1>
			<h1>dfasdfasdfa</h1>
			<h1>dfasdfasdfa</h1>
			<h1>dfasdfasdfa</h1>
		</Scroll>
	</div>
</template>

<script>
	import axios from "axios"
	import Scroll from "../components/Scroll.vue"

	var _this = null;
	export default {
		components: {
			Scroll
		},
		data() {
			return {}
		},
		beforeCreate() {
			_this = this;
		},
		created() {
			console.log(axios);
			console.log(_this);
		},
		methods: {
			onScrollUpPullEvent() {
				console.log("on scroll upPullEvent");
			},
			onScrollDownPullEvent() {
				console.log("on scroll down refresh");
			}
		}
	}
</script>

<style scoped>
	.homeMobileDiv {
		width: 100%;
		height: 100%;
	}

	.scroll {
		height: 100%;
	}
</style>
