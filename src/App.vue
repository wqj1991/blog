<template>
	<div id="app">
		<Layout>
			<div class="container">
				<Header class="nav">
					<div class="nav-inner">
						<router-link to="/" class="nav-title"> WYNNYO BLOG</router-link>
						<router-link to="/" class="nav-item"> <a-icon type="home" />首页</router-link>
						<router-link class="nav-item" to="/about"><a-icon type="appstore" />分类</router-link>
						<router-link class="nav-item" to="/about"><a-icon type="gift" />归档</router-link>
						<router-link class="nav-item" to="/about"><a-icon type="tags" />标签</router-link>
						<router-link class="nav-item" to="/about"><a-icon type="github" />开源</router-link>
						<router-link class="nav-item" to="/about"><a-icon type="meh" />关于</router-link>
					</div>
				</Header>
				<Content>
					<router-view />
				</Content>
				<Footer
					><a-icon type="copyright" />2020&nbsp;
					<a-icon type="heart" />
					&nbsp;wynnyo&nbsp;|&nbsp;赞赏</Footer
				>
			</div>
		</Layout>
	</div>
</template>

<style lang="less">
#app {
	font-family: 'Lato', 'PingFang SC', 'Microsoft YaHei', sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	text-align: center;
	color: #2c3e50;
}

.container {
	width: 100%;
}

.nav {
	padding: 30px;
	font-size: 12px;
	background: #2c3e50;
	height: 85px;
	.nav-inner {
		margin: auto;
		background: #2c3e50;
		max-width: 700px;
		text-align: right;
	}
	.nav-title {
		font-size: 22px;
		float: left;
	}
	.nav-item {
		margin-top: 20px;
		color: #fff;
		display: inline-block;
		padding-right: 10px;
		width: 68px;
		height: 26px;
		line-height: 26px;
		i {
			display: inline-block;
			margin: 0 10px;
		}
	}
	.nav-item:hover {
		color: #000;
		background: #fff;
	}
}

footer {
	background: #2c3e50;
	font-size: 14px;
	font-weight: 600;
	color: #fff;
	height: 50px;
	line-height: 50px;
	bottom: 0;
	position: absolute;
	width: 100%;
}
</style>
