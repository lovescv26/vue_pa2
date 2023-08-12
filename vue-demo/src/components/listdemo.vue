<template>
	<h3> 列表render </h3>
	<p v-for="item in name"> {{ item }} </p>
	<h4> ---- </h4>
	<div v-for="item in result">
		<p>  {{item.title}} </p>
		<a :href="item.avator">link </a>

	</div>
	<h4> ----key attritube put v-for </h4>
	<div v-for="item of result" :key="item.id">
	<!-- Im not sure why cant look key id?" -->
		<p>{{item.title}}</p>
		<a :href="item.avator"> link new in 0811 </a>
		</div>

	<h4>--- item and index--- </h4>
	<p v-for="(item,index) of name"> {{ item }} ~ {{index }} </p>
	<!-- in like python    of like javascript -->
	<h4 > --- item every index-key-value----</h4>
	<div>
		<p v-for="item of userinfo"> {{ item }} </p>
		<p v-for="(item,key,index)  of userinfo"> {{ item }}-{{key }} --{{ index}} </p>
	</div>

</template>
<script>
	export default{
		data(){
			return{
				name:["百戰","漫書","離火"],
				result:[
				{
					"id":520,
					"title": "我好想阿賢",
					"avator": "https://google.com",
				},
				{
					"id":1314,
					"title": "雖然阿賢很渣又過份",
					"avator": "https://www.bilibili.com/video/BV1Rs4y127j8?p=9&vd_source=ffaf28ca284a9a401200a7ddb40a906e",
				},
				{
					"id":1,
					// didnt use 0000 because 000 it not number ?@??@ i just want like zero
					"title": "08/07  12:58   阿賢 消失 23分鐘",
					"avator": "https://www.youtube.com/shorts/WxbIevN9nNY",
				},
				],
				userinfo:{
					name:"lumesen",
					age:20,
					height:169,

				}


			}
		}
	}

</script>
