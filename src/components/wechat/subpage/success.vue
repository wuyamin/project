<template>
	<div class="success">
		<img src="../../../assets/img/wechat/product/succeed.png"/>
		<p class="ding">订单提交成功</p>
		<p class="chu">出借处理中</p>
		<div class="success_btn clearfix">
			<span class="fl btn-left" @click="kanFun()">查看详情</span>
			<span class="fr btn-right" @click="chuFun()">继续出借</span>
		</div>
　　    </div>
</template>

<script>
	import { formatDate } from '../../../assets/js/wechat/date.js';
	import reset_rem from "../../../assets/js/wechat/reset_rem.js";
	export default {
        data () {
            return {
				items:[],
				baseEarnings: '',
				lcqx: '',
				fxfs: '',
				jiangLiEarnings: '',
				annualEarnings: '',
            };
        },
//      created: function () {
//      	this.$router.push({name:'go_invest',query:{ productId: this.productId }});
//      },
        methods: {
        	chuFun: function () {
        		this.$router.push({ path: 'product' });
        	},
        	kanFun: function () {
        		this.$router.push({ path: 'zeek_rewards' });
        	}
        }
    }
</script>

<style lang="less" scoped>
	@import url("../../../assets/css/wechat/reset_rem.css");
	@import url("../../../assets/css/wechat/success.less");
</style>