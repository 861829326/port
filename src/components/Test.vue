<template>
	<div class="test">
		<!--获取数据的方法-->
		<h1 class="ddd">{{title}}</h1>
		<!--获取对象的两种方法-->
		<p>{{user.firstName}}</p>
		<p v-text="user.lastName"></p>
		
		<!-- v-if -->
		<p v-if="showName">{{user.firstName}}</p>
		
		<!-- v-else -->
		<p v-else="showName">Nobady</p>
		
		<!--  v-for -->
		<ul>
			<li v-for="item in items">{{item}}</li>
		</ul>
	</div>
		
</template>

<script>
	export default {
 	 name: 'test',
 	 data() {
 	 	return {
 	 		title:"hello vue.js",
 	 		user:{
 	 			firstName:"hemiah",
 	 			lastName:"wu"
 	 		},
 	 		showName:false,
 	 		items:[
 	 				{title:"item 1"},
 	 				{title:"item 2"},
 	 				{title:"item 3"}
 	 		]
 	 	}
 	 }
}
</script>

<style>
	.ddd {
		color: red;
	}
</style>