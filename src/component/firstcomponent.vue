<template>
	<div id="firstcomponent">
		<h1>Component Title</h1>
		<a>Written by {{ author }}</a>
	</div>
</template>

<script>
	export default {
		data () {
			return {
				author: "liqiyuan"
			}
		}
	}
</script>

<style>
	body{
		font-family: "Microsoft Yahei";
	}
</style>