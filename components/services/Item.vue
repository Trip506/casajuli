<template>
	<div class="service">
		<div class="icon">
			<img :src="require('@/assets/image' + index + '.jpeg')" alt="" />
		</div>
		<h3>{{ title }}</h3>
		<p>
			Lorem ipsum, dolor sit amet consectetur adipisicing elit. Harum omnis nemo
			sapiente in quidem sed dolores cumque! Ut, est aliquid!
		</p>
	</div>
</template>

<script>
export default {
	props: ["index", "title"],
};
</script>