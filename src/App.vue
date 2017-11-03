<!-- 一个template（组件）下只能有一个并列的div -->
<template>
<div id="app">
	<img src="./assets/logo.png">
	<h1>{{ msg }}</h1>
	<firstcomponent></firstcomponent>
	<ul>
		<li><router-link to="/first">点我跳转到第一页</router-link></li>
		<li><router-link to="/second">点我跳转到第二页</router-link></li>
	</ul>
	<router-view class="view"></router-view>
</div>
</template>



<script>
import firstcomponent from './component/firstcomponent.vue'
import secondcomponent from './component/secondcomponent.vue'
export default {
	name: 'app',
	data () {
		return {
			msg: 'Welcome to Your Vue.js App'
	    }
	},
	components: { firstcomponent, secondcomponent }
}
</script>


<style>
body {
	font-family: Helvetica, sans-serif;
}
</style>
