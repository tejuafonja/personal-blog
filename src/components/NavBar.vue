<template>
	<div class="navbar">
		<ul class="navbar__links">
			<g-link to="/">Home</g-link>
			<g-link to="/xhirot">Xhirot</g-link>
			<!-- <a href="https://tejuafonja-projects.netlify.app/">Projects</a> -->
			<a href="https://scholar.google.com/citations?hl=en&user=u6q18aAAAAAJ/" target="_blank">Publications</a>
			<!-- <a href="https://sautiproject.com/" target="_blank">SautiProject</a> -->
            
		</ul>

	</div>
</template>


<style lang="scss">
.navbar {
	margin: 0 auto;
	max-width: 500px;
	text-align: center;

	&__image {
		border-radius: 100%;
		width: 90px;
		height: 90px;
		margin-bottom: 1em;
	}

	&__intro {
		opacity: .8;
	}

	&__site-title {
		margin: 0 auto;
		font-size: 1.5em;
		max-width: 400px;
	}

	&__links {
		margin: 0;
		a {
			margin: 0 .5em;
		}
	}
}
</style>
