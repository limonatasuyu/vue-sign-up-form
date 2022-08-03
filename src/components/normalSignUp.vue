<template>
	<div class="normalSignUp-container flex">
		<div>
			<form class="normalSignUp-wrapper grid">
				<h1>Sign Up</h1>
				<h2>Get started absolutely free</h2>
					<label class="text-label" for="email-input">Email</label>
					<input v-model='email' type="email" id="email-input" class="text-input" />
				
					<label class="text-label" for="password-input">Password</label>
					<input v-model='password' type="password" id="password-input" class="text-input" />

					<div class="checkbox-container flex">
						<input @click='toggleCheckBox' type="checkbox" id="terms-checkbox">
						<label for="terms-checkbox" >Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet</label>
					</div>
					<button @click.prevent='handleLogin' class="sign-up-button button">
						Sign up
					</button>
			</form>
		</div>
	</div>
</template>

<script>
export default {
	name: 'normalSignup',
	data() {
		return {
			email: '',
			password: '',
			isChecked: false
		}
	},
	methods: {
		handleLogin() {
			if (this.email.length === 0 || this.password.length === 0 || !this.isChecked) {alert('please fill the boxes'); return}
			console.log('email:', this.email, ' password:',this.password);
			this.email = '', this.password = ''},
		toggleCheckBox() {this.isChecked = !this.isChecked}
	}
}
</script>
