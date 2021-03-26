<template>
	<div>
		<div class="item">
			<img :src="require('@/assets/image' + index + '.jpeg')" alt="" />
			<div class="action">
				<a href="#">Launch</a>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	props: ["index"],
};
</script>

<style lang="css">
h2 p {
	color: white;
}
</style>