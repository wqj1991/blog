<template>
	<div id="app">
		<Layout>
			<div class="container">
				<Header class="nav">
					<div class="nav-inner">
						<router-link to="/" class="nav-title">王庆军的博客</router-link>
						<router-link to="/" class="nav-item"> <a-icon type="home" />首页 </router-link>
						<router-link class="nav-item" to="/about"> <a-icon type="appstore" />分类 </router-link>
						<router-link class="nav-item" to="/about"> <a-icon type="gift" />归档 </router-link>
						<router-link class="nav-item" to="/about"> <a-icon type="tags" />标签 </router-link>
						<router-link class="nav-item" to="/about"> <a-icon type="github" />开源 </router-link>
						<router-link class="nav-item" to="/about"> <a-icon type="meh" />关于 </router-link>
					</div>
				</Header>
				<Content>
					<div style="height:80px; width: 100%"></div>
					<router-view />
				</Content>
				<Footer> <a-icon type="copyright" />2020&nbsp; <a-icon type="heart" />&nbsp;wynnyo&nbsp;|&nbsp;赞赏 </Footer>
			</div>
		</Layout>
	</div>
</template>

<style lang="less">
body {
	position: relative;
	font-family: 'Lato', 'PingFang SC', 'Microsoft YaHei', sans-serif;
	font-size: 14px;
	line-height: 2;
	color: #555;
	background: #fff;
}
h1,
h2,
h3,
h4,
h5,
h6 {
	margin: 20px 0 10px;
}

p {
	margin: 0 0 25px 0;
	font-size: 16px;
	line-height: 2rem;
	color: #555;
}

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

.container > header {
	padding: 30px;
	font-size: 12px;
	background: #2c3e50;
	height: 85px;
	.nav-inner {
		margin: auto;
		background: #2c3e50;
		max-width: 900px;
		text-align: right;
	}
	.nav-title {
		font-size: 22px;
		float: left;
		font-weight: 700;
		color: #fff;
		margin-left: -15px;
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

.container > content {
	width: 100%;
	display: block;
	min-height: calc(100vh - 135px);
}

.container > footer {
	background: #2c3e50;
	font-size: 14px;
	font-weight: 600;
	color: #fff;
	height: 50px;
	line-height: 50px;
	width: 100%;
}
</style>
