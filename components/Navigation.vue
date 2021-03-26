<template>
	<div>
		<div class="toggle" @click="showNav = !showNav"></div>
		<div class="navigation active" v-show="showNav">
			<ul @click="showNav = !showNav">
				<li><a href="#home">Home</a></li>
				<li><a href="#services">Services</a></li>
				<li><a href="#work">Work</a></li>
				<li><a href="#contact">Contact</a></li>
			</ul>
			<!-- <div class="social-bar">
                        <ul>
                            <div v-for="(item, index) in 5" :key="index">
                                <li>
                                    <socialbaritem
                                        v-for="(item, index) in 5"
                                        :key="index"
                                        :index="index"
                                    ></socialbaritem>
                                </li>
                            </div>
                        </ul>
                    </div> -->
			<div class="social-bar">
				<ul>
					<li>
						<a href="https://facebook.com">
							<img
								src="https://github.com/bradtraversy/creative-agency-website/blob/master/images/facebook.png?raw=true"
								target="_blank"
								alt=""
							/>
						</a>
					</li>
					<li>
						<a href="https://twitter.com">
							<img
								src="https://github.com/bradtraversy/creative-agency-website/blob/master/images/twitter.png?raw=true"
								target="_blank"
								alt=""
							/>
						</a>
					</li>
					<li>
						<a href="https://instagram.com">
							<img
								src="https://github.com/bradtraversy/creative-agency-website/blob/master/images/instagram.png?raw=true"
								target="_blank"
								alt=""
							/>
						</a>
					</li>
				</ul>
				<a href="mailto:you@email.com" class="email-icon">
					<img
						src="https://github.com/bradtraversy/creative-agency-website/blob/master/images/email.png?raw=true"
						alt=""
					/>
				</a>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	data() {
		return {
			showNav: false,
		};
	},
	methods: {
		showNav() {},
	},
};
</script>

<style lang="css" scope>
/* NAVIGATION */
.toggle {
	cursor: pointer;
	position: fixed;
	top: 0;
	right: 0;
	width: 60px;
	height: 60px;
	background: var(--main-color)
		url("https://github.com/bradtraversy/creative-agency-website/blob/master/images/menu.png?raw=true");
	background-position: center;
	background-repeat: no-repeat;
	background-size: 30px;
	z-index: 20;
}

.toggle.active {
	background: var(--main-color)
		url("https://github.com/bradtraversy/creative-agency-website/blob/master/images/close.png?raw=true");
	background-position: center;
	background-repeat: no-repeat;
	background-size: 25px;
}

.navigation {
	position: fixed;
	top: 0;
	left: 100%;
	width: 100%;
	height: 100%;
	background-color: #fff;
	z-index: 15;
	display: flex;
	justify-content: center;
	align-items: center;
}

.navigation.active {
	left: 0;
}

.navigation ul {
	position: relative;
	list-style-type: none;
}

.navigation ul li {
	position: relative;
	text-align: center;
	padding-bottom: 5px;
}

.navigation ul li a {
	font-size: 2rem;
	color: var(--text-color);
	text-decoration: none;
	font-weight: 300;
}

.navigation ul li a:hover {
	color: var(--main-color);
}

.navigation .social-bar {
	position: absolute;
	top: 0;
	left: 0;
	width: 60px;
	height: 100%;
	display: flex;
	justify-content: center;
	align-items: center;
}

.navigation .social-bar a {
	display: inline-block;
	transform: scale(0.5);
}

.navigation .email-icon {
	position: absolute;
	bottom: 20px;
}
</style>