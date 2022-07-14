<template>
	<div id="faq" class="view">
		<div class="view-container">
			<div class="stripe">
				<div id="faq-content" class="stripe-content normal-text">
					<div class="align-left">
						<h2>About / FAQ</h2>
					</div>
					<div class="align-left">
						<div class="qa">
							<h3>
								I accidentally quit my browser. How do I rejoin an in-progress game?
							</h3>
							<p>Join the room again with your username exactly as it was.</p>
						</div>
						<div class="qa">
							<h3>My browser says my connection is not secure. Should I be concerned?</h3>
							<p>
								The reason you are getting this warning is because the site is currently hosted for free on Heroku without a paid SSL certificate.<br>
								This warning is less "there's a big shark in the water with you, get out" and more "your windows are open, maybe don't walk around naked".<br>
								As a general rule you should not enter sensitive information on a page with a "Not Secure" warning.<br>
								Sensitive information includes credit card numbers, full names, date of birth, and addresses.<br>
								Since we are not entering these things, a "Not secure" connection is safe for the purpose of playing the game.
							</p>
						</div>
						<div class="qa">
							<h3>Credits/Disclaimer</h3>
							<p>FAO is not affiliated with Oink Games.</p>
							<p>
								Notification SFX from
								<a href="https://material.io/design/sound/sound-resources.html"></a>
								(<a href="https://creativecommons.org/licenses/by/4.0/">CC-BY 4.0</a
								>)
							</p>
						</div>
					</div>
					<div class="align-right">
						<button class="btn secondary" @click="back()">OK</button>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
import Store from './state';
import VIEW from './view';
export default {
	name: 'RulesView',
	methods: {
		back() {
			Store.setView(VIEW.HOME);
		},
	},
};
</script>
