<template>
	<div>
		<header>
			<div class="logo">
				<h1>
					Hi, my name is Juli <br />
					I'm an investor, software engineer and crypto specialist
				</h1>
			</div>

			<Navigation></Navigation>
		</header>
		<!-- home -->
		<section class="home" id="home">
			<img :src="require('@/assets/profile.png')" class="home-img" alt="" />
			<div class="home-content">
				<img class="section-logo" :src="require('@/assets/logo1.svg')" alt="" />
				<h2>
					I help <span class="highlight">you</span> to achieve <br />
					<span class="highlight">your goals</span>
				</h2>

				<p>
					Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
					eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad
					minim veniam, quis nostrud exercitation ullamco laboris nisi ut
					aliquip ex ea commodo consequat. Duis aute irure dolor in
					reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla
					pariatur. Excepteur sint occaecat cupidatat non proident, sunt in
					culpa qui officia deserunt mollit anim id est laborum
				</p>

				<p>
					Software Engineer with experience in all levels of testing, including
					performance, functional, integration, system, regression, and user
					acceptance testing. Supportive and enthusiastic team player dedicated
					to streamlining processes and efficiently resolving project issues.
				</p>
				<br />
				<ul>
					<li>
						Investigation, design, and implement scalable applications for data
						identification, analysis, retrieval, and indexing
					</li>
					<li>
						Software design and development while remaining concentrate on
						client needs
					</li>
					<li>
						Cooperate diligently with other IT team members to plan, design, and
						develop smart solutions
					</li>
					<li>Estimate interface between hardware and software</li>
				</ul>
				<a href="#services" class="btn">Get Started</a>
			</div>
		</section>
		<!-- services -->
		<section id="services">
			<img class="section-logo" :src="require('@/assets/logo2.svg')" alt="" />
			<div class="title">
				<h1>Experience</h1>
			</div>

			<div class="services">
				<div v-for="(item, index) in 6" :key="index">
					<serviceitem :index="index" :title="items[index]"></serviceitem>
				</div>
			</div>
		</section>
		<!-- work -->
		<section id="work">
			<div class="title">
				<img
					class="section-logo"
					:src="require('@/assets/logomark.svg')"
					alt=""
				/>
				<h1>Some of our finest work</h1>
				<p>
					Cooperate diligently with other IT team members to plan, design, and
					develop smart solutions. Estimate interface between hardware and
					software. Interface with business analysts, developers, and technical
					support to determine optimal specifications.
				</p>

				<p>
					Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
					eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad
					minim veniam, quis nostrud exercitation ullamco laboris nisi ut
					aliquip ex ea commodo consequat. Duis aute irure dolor in
					reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla
					pariatur. Excepteur sint occaecat cupidatat non proident, sunt in
					culpa qui officia deserunt mollit anim id est laborum
				</p>
			</div>

			<div class="portfolio">
				<div v-for="(item, index) in 5" :key="index">
					<portfolioitem :index="index"></portfolioitem>
				</div>
			</div>
		</section>
		<!-- contact -->
		<section id="contact">
			<img
				class="section-logo"
				:src="require('@/assets/logomark1.svg')"
				alt=""
			/>
			<div class="title">
				<h2>Contact me</h2>
				<p>
					Lorem ipsum dolor, sit amet consectetur adipisicing elit. Doloribus
					iusto molestias accusamus rem nobis est, et laborum harum doloremque
					nemo non, minima quos totam labore
				</p>
			</div>

			<div class="contact">
				<div class="contact-form">
					<form>
						<div class="row">
							<div class="input50">
								<input type="text" placeholder="First Name" />
							</div>
							<div class="input50">
								<input type="text" placeholder="Last Name" />
							</div>
						</div>
						<div class="row">
							<div class="input50">
								<input type="text" placeholder="Email" />
							</div>
							<div class="input50">
								<input type="text" placeholder="Subject" />
							</div>
						</div>
						<div class="row">
							<div class="input100">
								<textarea placeholder="Message"></textarea>
							</div>
						</div>
						<div class="row">
							<div class="input100">
								<input type="submit" value="Send" />
							</div>
						</div>
					</form>
				</div>

				<!-- Map -->

				<div style="width: 100%">
					<iframe
						width="100%"
						height="600"
						frameborder="0"
						scrolling="no"
						marginheight="0"
						marginwidth="0"
						src="https://maps.google.com/maps?width=100%25&amp;height=600&amp;hl=en&amp;q=Tirana+(University%20of%20Tirana)&amp;t=&amp;z=14&amp;ie=UTF8&amp;iwloc=B&amp;output=embed"
					></iframe>
					>
				</div>
				<div class="contact-info">
					<div class="info-box">
						<img
							src="https://github.com/bradtraversy/creative-agency-website/blob/master/images/address.png?raw=true"
							class="contact-icon"
							alt=""
						/>
						<div class="details">
							<h4>Address</h4>
							<p>28 Rruga Borshi-Angleze, Tirana, Albania</p>
						</div>
					</div>
					<div class="info-box">
						<img
							src="https://github.com/bradtraversy/creative-agency-website/blob/master/images/email.png?raw=true"
							class="contact-icon"
							alt=""
						/>
						<div class="details">
							<h4>Email</h4>
							<a href="mailto:anyone@example.com">juli@juli-tourism.com</a>
						</div>
					</div>
					<div class="info-box">
						<img
							src="https://github.com/bradtraversy/creative-agency-website/blob/master/images/call.png?raw=true"
							class="contact-icon"
							alt=""
						/>
						<div class="details">
							<h4>Call</h4>
							<a href="tel:+19785555555">+1 978 555 5555</a>
						</div>
					</div>
				</div>
			</div>
		</section>
		<!-- Certificates -->
		<section>
			<div>
				<img width="300px" :src="require('@/assets/ielts.png')" alt="" />
				<img width="160px" :src="require('@/assets/tirana.png')" alt="" />
				<img width="300px" :src="require('@/assets/mit.png')" alt="" />
			</div>
		</section>
	</div>
</template>

<script>
export default {
	components: {
		Lightbox: () => import("@/components/Lightbox"),
		Navigation: () => import("@/components/Navigation"),
		serviceitem: () => import("@/components/services/Item"),
		portfolioitem: () => import("@/components/portfolio/Item"),
		socialbaritem: () => import("@/components/socialbar/Item"),
	},

	data() {
		return {
			title: "Juli Borsh professional care",

			items: [
				"Software Engineer",
				"International Investor",
				"Crypto Currency Consultant",
				"University Academic",
				"Professional Drone Pilot",
				"Electrictian",
				"Permaculture Gardener",
				"Home Maintenance Specialist",
				,
				"",
			],
		};
	},
};
</script>

<style lang="css">
@import url("https://fonts.googleapis.com/css2?family=Rubik:wght@300;500;700&display=swap");

:root {
	--main-color: #f60f20;
	--secondary-color: #1b206e;
	--highlight-color: #c4a2fc;
	--text-color: #111;
}

.section-logo {
	margin: 15px;
	width: 150px;
}

* {
	box-sizing: border-box;
	margin: 0;
	padding: 0;
}

html,
body {
	font-family: "Rubik", sans-serif;
	color: var(--text-color);
	scroll-behavior: smooth;
}

.btn {
	cursor: pointer;
	display: inline-block;
	background-color: var(--main-color);
	color: #fff;
	font-size: 1.1rem;
	text-decoration: none;
	padding: 10px 30px;
	margin: 20px 0;
	border: 0;
}

.btn:hover {
	transform: scale(0.98);
}

.logo {
	position: absolute;
	top: 16px;
	left: 40px;
	z-index: 20;
}

.logo h1 {
	font-size: 1.6rem;
	font-weight: 700;
}

/* SECTIONS */
section {
	display: flex;
	flex-direction: column;
	min-height: 100vh;
	align-items: center;
	padding: 100px 40px;
	margin-top: 60px;
}

h1 {
	font-size: 3rem;
	font-weight: 700;
}
h2 {
	font-size: 2rem;
	font-weight: 500;
}

p {
	margin: 20px 0 10px;
	font-size: 1.2rem;
	line-height: 1.5;
	font-weight: 300;
}

/* HOME SECTION */
section.home {
	flex-direction: row;
	margin-top: 0;
}

.home-content {
	position: relative;
	z-index: 10;
	max-width: 1000px;
}

/* Reference: https://stackoverflow.com/questions/43683187/how-can-i-create-custom-underline-or-highlight-for-text-in-html-or-css */
.highlight {
	background: linear-gradient(
		180deg,
		rgba(255, 255, 255, 0) 50%,
		var(--highlight-color) 50%
	);
	padding: 0 0.25rem;
}

.home-img {
	display: none;
}

/* SERVICES */
.services {
	margin-top: 40px;
	display: grid;
	grid-template-columns: 1fr;
	gap: 40px;
	text-align: center;
}

.services .service .icon img {
	max-width: 100px;
}

.services .service {
	padding: 30px;
	box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
}

.services .service h3 {
	font-size: 1.6rem;
	font-weight: 500;
	margin-top: 20px;
	color: var(--secondary-color);
}

.services .service p {
	line-height: normal;
	font-size: 1.1rem;
	margin: 10px 0;
}

/* WORK */
.portfolio {
	display: flex;
	justify-content: center;
	flex-wrap: wrap;
	margin-top: 20px;
}

.portfolio .item {
	position: relative;
	width: 300px;
	height: 300px;
	margin: 5px;
}

.portfolio .item img {
	width: 100%;
	height: 100%;
}

.portfolio .item .action {
	position: absolute;
	top: 0;
	left: 0;
	width: 100%;
	height: 100%;
	background-color: rgba(0, 0, 0, 0.8);
	display: flex;
	justify-content: center;
	align-items: center;
	opacity: 0;
	transition: opacity 0.5s ease-in-out;
}

.portfolio .item .action a {
	display: inline-block;
	color: #fff;
	text-decoration: none;
	border: 1px solid #fff;
	padding: 5px 15px;
}

.portfolio .item .action:hover {
	opacity: 1;
}

/* CONTACT */
.contact {
	position: relative;
	width: 100%;
	margin-top: 50px;
	display: flex;
	justify-content: space-between;
	align-items: flex-start;
	flex-direction: column;
}

.contact-form {
	position: relative;
	background-color: #f9f9f9;
	width: 100%;
	padding: 30px 30px 20px;
}

.contact-form form {
	width: 100%;
}

.contact-form .row {
	display: flex;
	flex-direction: column;
	width: 100%;
}

.contact-form .input50,
.contact-form .input100 {
	width: 100%;
	margin: 0;
}

.contact-form .row input,
.contact-form .row textarea {
	position: relative;
	border: 1px solid rgba(0, 0, 0, 0.2);
	color: #111;
	background: transparent;
	width: 100%;
	padding: 10px;
	outline: none;
	font-size: 1rem;
	font-family: inherit;
	font-weight: 300;
	margin: 10px 0;
	resize: none;
}

.contact-form .row textarea {
	height: 150px;
}

.contact-form .row input[type="submit"] {
	background-color: var(--secondary-color);
	color: #fff;
	margin: 0;
	text-transform: uppercase;
	letter-spacing: 2px;
	font-weight: 300;
	border: 0;
	cursor: pointer;
}

.contact-info {
	width: 100%;
	margin-top: 20px;
	background: #f9f9f9;
	padding: 30px 30px 20px;
}

.contact-info .info-box {
	display: flex;
	align-items: flex-start;
	margin-bottom: 40px;
}

.contact-info .info-box .contact-icon {
	width: 20px;
	margin-right: 40px;
}

.contact-info .info-box .details h4 {
	color: var(--secondary-color);
}

.contact-info .info-box .details p,
.contact-info .info-box .details a {
	color: var(--text-color);
}

/* MEDIA QUERIES */
@media (min-width: 768px) {
	.services {
		grid-template-columns: repeat(2, 1fr);
	}

	.services .service {
		box-shadow: none;
	}

	.services .service:hover {
		box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
	}
}

@media (min-width: 1068px) {
	.home-img {
		display: block;
		position: absolute;
		bottom: 0;
		right: 0;
		height: 110%;
	}

	.logo {
		top: 30px;
		left: 100px;
	}

	.logo h1 {
		font-size: 2.1rem;
	}

	.navigation ul li a {
		font-size: 2.3rem;
	}

	section {
		padding: 100px;
	}

	.services {
		grid-template-columns: repeat(3, 1fr);
	}

	.contact {
		flex-direction: row;
	}

	.contact-form {
		width: calc(100% - 400px);
		padding: 60px 40px 20px;
	}

	.contact-form .row {
		flex-direction: row;
	}

	.contact-form .input50 {
		width: 50%;
		margin: 0 10px;
	}

	.contact-form .input100 {
		margin: 0 10px;
	}

	.contact-info {
		width: 350px;
		margin-top: 0;
		padding: 60px 40px 20px;
	}
}
</style>