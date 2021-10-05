<template>
	<div class="serie">
		<img class="serie__image" :src="ser.thumb" :alt="ser.title">
		<div class="product__name">
			{{ser.title}}
		</div>
	</div>
</template>

<script>
export default {
	name: "Serie",
	props: ['ser']
}
</script>



<style lang="scss" scoped>
	.serie{
		width: calc(100% / 6);
		height: 15rem;
		padding: 2.1875rem 10px;
		color: #fff;
		.serie__name{
			text-align: center;
			font-weight: 500;
			width: 60%;
			margin: 0 auto;
		}
		.serie__image{
			width: 100%;
			height: 100%;
			object-fit: cover;
			object-position: top;
		}
	}
</style>