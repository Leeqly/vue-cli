<template>
	<div id="second-page">
		<h1>I am the second page</h1>
		<a>written by {{ author }}</a>
		<p>{{ article }}</p>
	</div>
</template>
 
<script>
export default {
	data() {
		return {
			author: "liqiyuan",
			article: '第二个子页面',
	    }
	}
}
</script>
 
<style>
</style>