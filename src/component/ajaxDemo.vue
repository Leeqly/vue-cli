<template>
	<div id="ajax-demo">
		<ul>
			<li v-for="list in people"> {{ list.name }} </li>
		</ul>
	</div>
</template>
 
<script>
	import axios from 'axios'
	export default{
		data(){
			return {
				people: []
			}
		},
		mounted: function(){
			axios.get('/src/data/ajaxDemo.json', {}).then( (response)=>{
				this.people = response.data.list;
			});
		}
	}
</script>
 
<style>
</style>