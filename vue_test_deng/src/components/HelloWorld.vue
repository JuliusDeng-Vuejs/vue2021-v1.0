<template>
	<div id="">

		<h2>黎海霞 是不是 小仙女？</h2>
		<ul>
			<li>A 是</li>
			<li>B 不是</li>
		</ul>
		<h3>很明显，我们选B</h3>
		<h2>邓宇辰 是帅气的小哥哥 哦 ？</h2>
		<ul>
			<li>A 是</li>
			<li>B 当然是</li>
		</ul>
		<h3>很明显，我们也选B</h3>



	</div>
</template>

<script>
	export default {
		name: 'HelloWorld',
		props: {
			msg: String
		}
	}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
	h3 {
		margin: 40px 0 0;
	}

	ul {
		list-style-type: none;
		padding: 0;
	}

	li {
		display: inline-block;
		margin: 0 10px;
	}

	a {
		color: #42b983;
	}
</style>
