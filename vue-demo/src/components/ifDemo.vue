<template>
	<h3> confident render </h3>
	<div v-if="flag" > U can see me? </div>
	<div v-else> i miss lumesen </div>
	<div v-if="type==='A'"> A </div>
	<div v-else-if="type==='B'"> B </div>
	<div v-else-if="type==='C'"> C </div>
	<div v-else> NOt A/B/C </div>
	<div v-show="flag"> show  </div>


</template>
<script>
	export default{
	data(){
		return{
			//flag:true,
			flag:false,
			type:"B",


		}
	}
	}

</script>
