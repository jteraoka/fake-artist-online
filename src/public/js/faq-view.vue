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
								I have some form of color blindness/color deficiency. Can I still play this game?
							</h3>
							<p>I selected the in-game color palette with accessibility as a priority. My hope is that each color will be distinguishable from the others while drawing, but I apologize if that ends up not being the case.</p>
						</div>
						<div class="qa">
							<h3>
								I accidentally quit my browser. How do I rejoin an in-progress game?
							</h3>
							<p>Join the room again with your username exactly as it was.</p>
						</div>
						<div class="qa">
							<h3>My browser says my connection is not secure. Should I be concerned?</h3>
							<p>The reason you are getting this warning is because the site is currently hosted for free on Heroku without a paid SSL certificate.</p>
							<p>This warning is less "there's a big shark in the water with you, get out" and more "your windows are open, maybe don't walk around naked".</p>
							<p>As a general rule you should not enter sensitive information on a page with a "Not Secure" warning. Sensitive information includes credit card numbers, passwords, full names, date of birth, and addresses.</p>
							<p>A "Not secure" connection is safe for the purpose of playing the game as long as you don't enter these things.</p>
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
