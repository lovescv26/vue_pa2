<template>
<h2> title </h2>

<p>
{{ msg }}
</p>
<h3>  this is number </h3>
<p> {{number + 101}} </p>
<p> {{ ok ? "test 3" : "neo" }} </p>
<p> {{ hello.split("").reverse().join("")}} </p>
<h3> ---- split----- </h3>
<p> {{rawhtml}} </p>
<p v-html="rawhtml"></p>

</template>
<script >
	export default{
		data(){
		return{
		msg : "magic love ",
		hello: "hello world ",
		number : 10,
		ok: true,
		rawhtml: "<a href='https://www.bilibili.com/video/BV1Rs4y127j8?p=6&vd_source=ffaf28ca284a9a401200a7ddb40a906e'> 愛情的 </a>"	

		}
		}
	}

</script>
