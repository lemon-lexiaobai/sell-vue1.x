<template>
	<div class="price">
		<span class="now">￥{{ price }}</span>
		<span class="old" v-show="oldPrice">￥{{ oldPrice }}</span>
	</div>
</template>

<script type="text/javascript">
	export default {
		props: {
			price: {
				type: Number
			},
			oldPrice: {}
		}
	};
</script>

<style lang='stylus' rel='stylesheet/stylus'>
	.price
		font-weight: 700
		line-height: 24px
		font-size: 0
		.now
			margin-right: 8px
			font-size: 14px
			color: rgb(240,20,20)
		.old
			text-decoration: line-through
			font-size: 10px
			color: rgb(147,153,159)
</style>
