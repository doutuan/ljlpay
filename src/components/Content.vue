<template>
  <div id="content" class="clearfix">
    <div id="navLeft" class="fl">
		<img src="../assets/img/logo_cricle.png" alt="" class="navLogo">
		<p class="name">{{userName}}</p>
      <ul class="navList">
        <li class="active">我的58汽配</li>
        <li>我的账户信息</li>
      </ul>
    </div>
    <div id="navRight" class="fl">
    	<loanInfo></loanInfo>
    </div>
  </div>
</template>

<script>
import LoanInfo from '../components/LoanInfo.vue'

export default {
  name: 'content',
  data () {
    return {
      userName: '外星来者'
    }
  },
  components: {
    'loanInfo': LoanInfo
  }
}
</script>

<style scoped>

#content{
  width: 1192px;
  height: 750px;
  margin:auto;
  background: #f5f5f5;
}
#navLeft{
	width: 210px;
	height: 100%;
	border:1px solid rgb(214, 218, 225);
	border-top: none;
	background: #eaeef4;
	padding-top: 44px;
	box-sizing: border-box;
	font-family: '微软雅黑';
}
.navLogo{
	width: 120px;
	height: 120px;
	margin:auto;
	display: block;
}
.name{
    font-size: 14px;
    color: #414141;
    text-align: center;
    padding: 20px;
}
.navList{
	width: 211px;
}
.navList li{
	width: 211px;
	height: 40px;
    line-height: 40px;
    padding-left: 20px;
    margin-top: 5px;
    box-sizing: border-box;
    font-size:16px;
    color:#646464;
    background: url(../assets/img/rightjian.png) no-repeat 156px 14px;
    background-size: 7px 12px;
    cursor: pointer;
}
.navList .active{
	background: url(../assets/img/rightjian.png) no-repeat 156px 14px #fff;
}
#navRight{
	width: 978px;
	height: 100%;
	background: #fff;
}
</style>
