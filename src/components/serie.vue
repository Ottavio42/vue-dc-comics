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
		border: 2px solid #dbe9ff;
		background-color: #fff;
		padding: 25px 0;
		.serie__name{
			text-align: center;
			font-weight: 500;
			width: 60%;
			margin: 0 auto;
		}
		.serie__image{
			width: 50px;
		}
	}