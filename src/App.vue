<script setup>
// import HomeNav from './components/home/HomeNav.vue'
import "bootstrap/dist/css/bootstrap.min.css"
import "bootstrap"
</script>

<template>
	<div container>
		<header class="row">
			<!-- <HomeNav></HomeNav> -->
			<div class="col">
				<span>JCL&YMJ</span>
			</div>
			<div class="navUl col">
				<ul class="ul-list col-6 list-inline">
					<li class="list-inline-item"><a href="#">首页</a></li>
					<li class="list-inline-item"><a href="#">博客文档</a></li>
					<li class="list-inline-item"><a href="#">JCL&YMJ</a></li>
					<li class="list-inline-item"><a href="#">关于我</a></li>
					<li class="list-inline-item"><a href="#">相册</a></li>
					<li class="list-inline-item"><a href="#">时间线</a></li>
				</ul>
			</div>
		</header>

		<main>

		</main>
	</div>

</template>
<script>
var _this;
export default {
	comments: {},
	data() {
		return {

		}
	},
	onLoad(e) {

	},
	onShow() {

	},

	methods: {

	}
}
</script>
<style>
/* 设置列表横排样式 */
header ul {
	display: inline-block;
}

/* 设置导航菜单靠右显示 */
.navUl {
	text-align: right;
}

/* 设置上方导航鼠标移上样式 */
header ul li a {
	text-decoration: none;
	color: aquamarine;
	
}
header ul li a:hover{
	animation-name: navalink;
	animation-duration: 1.5s;
}

/* 鼠标移上动画效果 */
@keyframes navalink {
	from {
		color: aquamarine;
	}
	50%{
		color: blue;
	}
	to {
		color: red;
	}
}
</style>
