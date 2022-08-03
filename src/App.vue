<template>
	<div id="app" class="app-container flex">
		<SocialSignUp />
		<NormalSignUp />
	</div>
</template>

<script>
import SocialSignUp from './components/socialSignUp.vue'
import NormalSignUp from './components/normalSignUp.vue'

export default {
	name: 'App',
	components: {
		SocialSignUp, NormalSignUp
	}
}
</script>
<style>
</style>
