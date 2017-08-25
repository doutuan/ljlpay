<template>
	<div id="loanInfo" class="clearfix">
		<div class="fl ">
			<div class="clearfix repaymentInfo">
				<div class="fl">
					<p class="hint">最近需还款本额</p>
					<p class="loanAmount">¥ {{amount}}</p>
					<div class="lineBox"></div>
					<p class="loanTime">最近需还款日期：{{time}}</p>
				</div>
				<input type="button" value="获取更高额度" class="fr limitIncrease">
			</div>
			<ul class="creditInfo clearfix ">
				<li class="fl">
					<h3 class="clearfix title">
						<p class="line fl"></p>
						<p class="fl">还款</p>
						<p class="line fl"></p>
					</h3>
					<p>全部未还订单总额</p>
					<span>¥ {{dueAmount}}</span>
					<span>未还订单笔数</span>
					<p>{{nopaySum}}</p>
				</li>
				<li class="fl">
					<h3 class="clearfix title">
						<p class="line fl"></p>
						<p class="fl">额度</p>
						<p class="line fl"></p>
					</h3>
					<p>可用余额</p>
					<span>¥ {{creditBalance}}</span>
					<span>授信总额度</span>
					<p>¥ {{creditSum}}</p>
				</li>
				<li class="fl">
					<h3 class="clearfix title">
						<p class="line fl"></p>
						<p class="fl">消费</p>
						<p class="line fl"></p>
					</h3>
					<p>累计消费总额</p>
					<span>¥ {{totalLoanAmount}}</span>
					<span>累计消费次数</span>
					<p>{{expendCount}}</p>
				</li>
				<li class="fl rightNone">
					<h3 class="clearfix title">
						<p class="line fl"></p>
						<p class="fl">提升</p>
						<p class="line fl"></p>
					</h3>
					<p>累计提升额度</p>
					<span>¥ {{enterpriseRiskMoney}}</span>
					<span>累计提额次数</span>
					<p>{{enterpriseRiskCount}}</p>
				</li>
			</ul>
		</div>
		
		<div class="creditScore fr">
			<h3 class="clearfix  creditTitle">
				<p class="line fl"></p>
				<p class="fl">信用分数</p>
				<p class="line fl"></p>
			</h3>
			<div class="torusImg">
				<div class="torus">
					<div class="subTorus">
						
					</div>
				</div>
			</div>
		</div>
	</div>
</template>
<style>
	#loanInfo{
		width: 890px;
		border:1px solid red;
		margin-left:50px;
		font-family: '微软雅黑';
	}
	.repaymentInfo{
		width: 660px;
	    color: #414141;
	    margin-top: 70px;
    	margin-bottom: 20px;
	}
	.hint{
		font-weight: bold;
	    font-size: 18px;
	}
	.loanAmount{
		font-family: helvetica;
		height: 34px;
		line-height: 34px;
		font-weight: bold;
	    font-size: 30px;
	}
	.lineBox{
		height: 8px;
	    width: 255px;
	    background: #eaeef4;
	}
	.loanTime{
	    font-size: 14px;
	    color: #646464;
	}
	.limitIncrease{
		width: 160px;
		height: 44px;
		line-height: 44px;
		margin-right: 30px;
	    border: 1px solid #eb5959;
	    -webkit-border-radius: 5px;
	    -moz-border-radius: 5px;
	    border-radius: 5px;
	    text-align: center;
	    color: #eb5959;
	    font-weight: bold;
	    background: none;
		cursor: pointer;
	}
	.creditInfo{

	}
	.creditInfo li{
		width: 150px;
	    height: 180px;
	    border: 1px solid #dddddd;
	    margin-right: 20px;
	    text-align: center;
	    font-style: 16px;
	    color: #646464;
	}
	.creditInfo .rightNone{
		margin-right: 0;
	}
	.title{
	    width: 110px;
	    height: 30px;
	    margin: 25px auto 0;
	}
	.line{
		width: 30px;
		height: 1px;
		background: #ddd;
		margin: 9px 5px;
	}
	.creditInfo li span{
		font-size: 14px;
		display: block;
		margin:5px 0;
	}
	.creditScore{
		height: 355px;
	    width: 210px;
	    border: 1px solid #cccccc;
	    border-top: 1px solid #fff;
	    color:#646464;
	}
	.creditTitle{
		width: 150px;
	    height: 30px;
	    margin: 25px auto 0;
	}
	.torusImg{
		height: 100px;
		overflow: hidden;
	}
	.torus{
		width: 170px;
		height: 170px;
		margin:auto;
		border:16px solid rgb(238, 238, 238);
		border-radius: 50%;
		position: relative;
	}
	.subTorus{
		width: 170px;
		height: 170px;
		margin:auto;
		border:16px solid #c9a161;
		border-radius: 50%;
		position: absolute;
		left:-16px;
		top:-16px;
	}
</style>
<script>
	export default {
	  data () {
	    return {
	      amount: '0',
	      time: '--',
	      dueAmount: '0.00',
	      nopaySum: '0',
	      creditBalance: '0.00',
	      creditSum: '0.00',
	      totalLoanAmount: '0.00',
	      expendCount: '0',
	      enterpriseRiskMoney: '0.00',
	      enterpriseRiskCount: '0'
	    }
	  }
	}
</script>