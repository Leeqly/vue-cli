<template>
	<div id="first-page">
		<h1>I am the first page</h1>
		<a>written by {{ author }}</a>
		<p>{{ article }}</p>
	</div>
</template>
 
<script>
export default {
	data() {
		return {
			author: 'liqiyuan',
			article: '第一个子页面',
	    }
	}
}
</script>
 
<style>
</style>