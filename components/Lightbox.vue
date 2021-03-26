<template>
	<div>
		<div class="cssbox">
			<a id="image1" href="#image1">
				<img class="cssbox_thumb" :src="require('@/assets/image1.jpeg')" />
				<span class="cssbox_full">
					<img :src="require('@/assets/image1.jpeg')" />
				</span>
			</a>
			<a class="cssbox_close" href="#void"></a>
			<a class="cssbox_next" href="#image2">&gt;</a>
		</div>

		<div class="cssbox">
			<a id="image1" href="#image2">
				<img class="cssbox_thumb" :src="require('@/assets/image2.jpeg')" />
				<span class="cssbox_full">
					<img :src="require('@/assets/image2.jpeg')" />
				</span>
			</a>
			<a class="cssbox_close" href="#void"></a>
			<a class="cssbox_prev" href="#image1">&lt;</a>
			<a class="cssbox_next" href="#image3">&gt;</a>
		</div>

		<div class="cssbox">
			<a id="image1" href="#image3">
				<img class="cssbox_thumb" src="thumbn-3.jpg" />
				<span class="cssbox_full">
					<img src="full-3.jpg" />
				</span>
			</a>
			<a class="cssbox_close" href="#void"></a>
			<a class="cssbox_prev" href="#image2">&lt;</a>
		</div>
	</div>
</template>

<style lang="css" scope>
/* The work below, CSSBox, is released under the Creative Commons
   Attribution-ShareAlike 4.0 license and is available on
   https://github.com/TheLastProject/CSSBox. You are not required to add
   additional credit to your website, just leave the above text in this file */
div.cssbox {
	display: inline-block;
}

span.cssbox_full {
	z-index: 999999;
	position: fixed;
	height: 100%;
	width: 100%;
	background-color: rgba(0, 0, 0, 0.8);
	top: 0;
	left: 0;
	opacity: 0;
	pointer-events: none;
	cursor: default;
	transition: opacity 0.5s linear;
}

span.cssbox_full img {
	position: fixed;
	background-color: white;
	margin: 0;
	padding: 0;
	max-height: 90%;
	max-width: 90%;
	top: 50%;
	left: 50%;
	margin-right: -50%;
	transform: translate(-50%, -50%);
	box-shadow: 0 0 20px black;
}

a.cssbox_close,
a.cssbox_prev,
a.cssbox_next {
	z-index: 999999;
	position: fixed;
	text-decoration: none;
	visibility: hidden;
	color: white;
	font-size: 36px;
}

a.cssbox_close {
	top: 1%;
	right: 1%;
}

a.cssbox_close::after {
	content: "\00d7";
}

a.cssbox_prev,
a.cssbox_next {
	top: 50%;
	transform: translate(0%, -50%);
}

a.cssbox_prev {
	left: 5%;
}

a.cssbox_next {
	right: 5%;
}

a:target ~ a.cssbox_close,
a:target ~ a.cssbox_prev,
a:target ~ a.cssbox_next {
	visibility: visible;
}

a:target > img.cssbox_thumb + span.cssbox_full {
	visibility: visible;
	opacity: 1;
	pointer-events: initial;
}
/* This is the end of CSSBox */
</style>