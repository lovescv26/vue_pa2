<template>
	<h3> ------- key attritube add to the v-for   ------</h3>
	<p v-for="(item,index) in names" :key="index" >{{ item }} </p>
	<!--  :key == v-bind  is special  -->
	<!-- but not recommand didn't do it ... because if 0 1 2 if you want put the value that prior array -->
	<!-- recommend use only one key "id" -->



</template>
<script>
	export default{
		data(){
			return{
				names:["0305的人","明明很理性","但是我卻好像動了凡心","我知道我完蛋了"]


			}
		}
	}

</script>
