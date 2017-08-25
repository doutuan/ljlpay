<template>
	<div id="head">
		<div class="headTop clearfix">
			<a class="wubaHome fl" href="http://59.110.12.113:9011/">58汽配网首页</a>
			<ul class="fr loginInfo">
				<li>{{userName}}</li>
				<li>退出</li>
				<li>联系电话 ： 010-1234-5678</li>
			</ul>
		</div>
		<div class="headBottom clearfix">
			<p class="fl">58汽配</p>
			<ul class="fr">
				<li class="money">无需任何实物抵押</li>
				<li class="credit ">授信额度循环使用</li>
				<li class="amount">额度可快速提升</li>
			</ul>
		</div>
	</div>
</template>
<style scoped>
	#head{
		width: 100%;
		height: 140px;
		background: #fff;
		border-bottom:1px solid rgb(214, 218, 225);
		font-family: "微软雅黑";
		color: #414141;
	}
	.headTop{
		height: 40px;
		line-height: 40px;
		background: #d7d7d7;
		font-size: 14px;
	}
	.wubaHome{
		line-height: 40px;
		margin-left: 13.3%;
		padding-left: 30px;
		background: url(../assets/img/header_house.png) no-repeat 0 7px;
		background-size: 24px 24px;
	}
	.loginInfo{
		margin-right: 171px;
	}
	.loginInfo li{
		float: left;
		margin-right: 14px;
	}
	.headBottom{
		height: 100px;
	}
	.headBottom p{
	    width: 176px;
	    font-size: 22px;
	    line-height: 100px;
	    margin-left: 12.1%;
	    padding-left: 186px;
	    background: url(../assets/img/topLogo_yuansheng.png) no-repeat 0 53%;
	    background-size: 144px 71px;
	}
	.headBottom ul{
		width: 630px;
		margin-right: 127px;
	}
	.headBottom ul li{
		float: left;
		padding-left: 40px;
		font-size: 18px;
		line-height: 100px;
		margin-right: 20px;
	}
	.money{
		background: url(../assets/img/header_rmb.png) no-repeat 0 36px;
		background-size: 30px 30px;
	}
	.credit{
		background: url(../assets/img/header_xin.png) no-repeat 0 36px;
		background-size: 30px 30px;
	}
	.amount{
		background: url(../assets/img/header_e.png) no-repeat 0 36px;
		background-size: 30px 30px;
	}
</style>
<script>
	export default {
	  name: 'Head',
	  data () {
	    return {
	      userName: '外星来者'
	    }
	  }
	}
</script>