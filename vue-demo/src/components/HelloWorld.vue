<template>
	<div v-bind:id="dynamicID"  :class="  msg " v-bind:title="dynamicTitle"    > test </div>
	<!-- look v-bind: == : -->
	<button :disabled="isbuttondisabled"> button</button>
	<div v-bind="objectOfattrs" > TT  </div>

</template>
<script >
	export default{
	data(){
		return{
		msg:"appclass",
		dynamicID:"appID",
		//dynamicTitle:null
		dynamicTitle:"haha",
		//isbuttondisabled:"false"
		// didnt ues double quote
		isbuttondisabled:false,
		objectOfattrs:{
		class:"appclass",
		id:"bananid",

		}

		}
	}
	}

</script>


<style>
.appclass{
	color: red;
	font-size: 30px;
}

</style>
