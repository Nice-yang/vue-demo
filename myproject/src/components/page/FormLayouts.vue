
<!--菜单-->
<template>
	<div>
		 <v-pageTitle vtitle="FormLayouts"></v-pageTitle>
		  <el-row>
            <el-col :span="24">
                <el-card class="box-card">
                    InlineForm-行布局
                    <hr>
                    <inlineForm></inlineForm>
                </el-card>
            </el-col>
        </el-row>

        <el-row :gutter="20">
            <el-col :xs="24" :sm="24" :md="8" :lg="8">
                <el-card class="box-card card-a">
                    Right Layout Form
                    <hr>
                    <rightlayoutForm></rightlayoutForm>
                </el-card>
            </el-col>
             <el-col :xs="24" :sm="24" :md="8" :lg="8">
                <el-card class="box-card card-a">
                    Left Layout Form
                    <hr>
                    <leftLayoutForm></leftLayoutForm>
                </el-card>
            </el-col>
             <el-col :xs="24" :sm="24" :md="8" :lg="8">
                <el-card class="box-card card-a">
                    Top Layout Form
                    <hr>
                    <topLayoutForm></topLayoutForm>
                </el-card>
            </el-col>
        </el-row>
	</div>
</template>
<script>
	import vPageTitle from '../common/pageTitle';
	import inlineForm from '../forms/inlineForm';
	import leftLayoutForm from '../forms/leftLayoutForm';
	import rightlayoutForm from '../forms/rightlayoutForm';
	import topLayoutForm from '../forms/topLayoutForm';
	export default {
		components:{
			vPageTitle,inlineForm,leftLayoutForm,rightlayoutForm,topLayoutForm
		},
		data(){
			return{
				
			}
		},
		methods:{
			
		}
	}
</script>