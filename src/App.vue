<script setup>
// import HomeNav from './components/home/HomeNav.vue'
import "bootstrap/dist/css/bootstrap.min.css"
import "bootstrap"
</script>

<template>
	<div container>
		<header class="row">
			<!-- <HomeNav></HomeNav> -->
			<div class="col-3">
				<span>JCL&YMJ</span>
			</div>
			<div class="navUl col-9">
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
	font-weight: 600;

}
/* 鼠标移上导航栏菜单后边框从中间展开 */
header ul li a {
	display: inline-block;
	line-height: 30px;
	padding: 0 10px;
	cursor: pointer;
	position: relative;
}
header ul li a::after {
	content: "";
	border-bottom: red solid 2px;
	display: block;
	transform: scale(0);
	transition: all 0.6s ease-out 0s;
}
header ul li a:hover::after {
	animation-direction: alternate;
	animation: navHover 1s 0s infinite linear;
}
	/* 鼠标移上导航栏菜单动画效果 */
@keyframes  navHover{
    0%{
		transform: scale(0);	
	}
	50%{
		transform: scale(1);
	}
    100%{
		transform: scale(0);
	}
}


</style>
