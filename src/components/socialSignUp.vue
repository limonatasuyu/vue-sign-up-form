<template>
	<div class="socialSignUp-container flex">
		<div class="socialSignUp-buttons-wrapper grid">
			<button v-for="i, x in socaialsList" :key="x" class="social-button button flex">
				<img class='social-logo' :src='logosList[x]' />
				<p>Sign up with {{i}}</p>
			</button>
		</div>
	</div>
</template>

<script>
import linkedInLogo from '../assets/img/LinkedInLogo.png'
import twitterLogo from '../assets/img/TwitterLogo.png'
import facebookLogo from '../assets/img/FacebookLogo.png'

export default {
	data() {
		return {
			socaialsList: ['Linkedin', 'Twitter', 'Facebook'],
			logosList: [linkedInLogo, twitterLogo, facebookLogo]
		}
	},
	name: 'socialSignUp'
}
</script>

<style>
</style>
