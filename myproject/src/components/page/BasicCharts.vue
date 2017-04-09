
<!--菜单-->
<template>
	<div>
		 <v-pageTitle vtitle="BasicCharts"></v-pageTitle>


        <el-row :gutter="20">
            <el-col :xs="24" :sm="24" :md="8" :lg="8">
                <el-card class="box-card">
                    <barChart></barChart>
                </el-card>
            </el-col>
            <el-col :xs="24" :sm="24" :md="8" :lg="8">
                <el-card class="box-card">
                    <lineChart></lineChart>
                </el-card>
            </el-col>
            <el-col :xs="24" :sm="24" :md="8" :lg="8">
                <el-card class="box-card">
                   <radarChart></radarChart>
                </el-card>
            </el-col>
        </el-row>

        <el-row :gutter="20">
            <el-col :xs="24" :sm="24" :md="12" :lg="12">
                <el-card class="box-card">
                    <pieChart></pieChart>
                </el-card>
            </el-col>
            <el-col :xs="24" :sm="24" :md="12" :lg="12">
                <el-card class="box-card">
                    <funnelChart></funnelChart>
                </el-card>
            </el-col>
            
        </el-row>
	</div>
</template>
<script>
	import vPageTitle from '../common/pageTitle';
	import barChart from '../echarts/barChart';
	import funnelChart from '../echarts/funnelChart';
	import lineChart from '../echarts/lineChart';
	import pieChart from '../echarts/pieChart';
	import radarChart from '../echarts/radarChart';
	export default {
		components:{
			vPageTitle,barChart,funnelChart,lineChart,pieChart,radarChart
		},
		data(){
			
		},
		methods:{
			
		}
	}
</script>
