
<!--菜单-->

<template>
    <div class="sidebar">
        <el-menu :default-active="onRoutes" class="el-menu-vertical-demo" theme="dark" unique-opened router>
            <el-menu-item index="DashBoard">
               
                    <span class="sb-icon"><i class="material-icons">home</i></span>
                    <span class="sb-cn">DashBoard</span>
            </el-menu-item>

            <el-submenu index="2">
                <template slot="title">
               
                    <span class="sb-icon"><i class="material-icons">perm_data_setting</i></span>
                    <span class="sb-cn">Components</span>
                 
                </template>
                <el-menu-item index="EditorPage">Editor</el-menu-item>
                <el-menu-item index="MarkdownPage">Markdown</el-menu-item>
                <el-menu-item index="TodoList">TodoList</el-menu-item>
                     
                
            </el-submenu>

            <el-submenu index="3">
                <template slot="title">
                    <span class="sb-icon"><i class="material-icons">pie_chart</i></span>
                    <span class="sb-cn">charts</span>
                </template>
                <el-menu-item index="BasicCharts"> BasicCharts</el-menu-item>
            </el-submenu>

            <el-submenu index="4">
                <template slot="title">
                    <span class="sb-icon"><i class="material-icons">content_paste</i></span>
                    <span class="sb-cn">Form Elements</span>
                </template>
                <el-menu-item index="FormInput"> Form Inputs</el-menu-item>
                <el-menu-item index="FormLayouts">  Form Layouts</el-menu-item>
            </el-submenu>

             <el-submenu index="5">
                <template slot="title">
                    <span class="sb-icon"><i class="material-icons">border_all</i></span>
                    <span class="sb-cn">Tables</span>
                </template>
                <el-menu-item index="BasicTables"> Basic Tables</el-menu-item>
                
            </el-submenu>        
        </el-menu>
    </div>
</template>
<script>
	
   export default{
   		data(){
   			return {
   				menus:[
   					{icon:'home',menuName:'Home',isActive:false},
   					{icon:'perm_data_setting',menuName:'Components',children:['Editor','Markdown','TodoList'],isActive:false},
   					{icon:'pie_chart',menuName:'charts',children:['BasicCharts'],isActive:false},
   					{icon:'border_all',menuName:'Tables',children:['Basic Tables'],isActive:false},
   					{icon:'content_paste',menuName:'Form Elements',children:['FormInputs','Form Layouts'],isActive:false}
   				]
   			}
   		},
		methods:{
			/*菜单动画选项卡*/
   			/*isOpen(index){
   				console.info(this.menus.length-1)
   				if(index != 0 && index <=4){
   					this.menus[(index-1)].isActive =false;
   					if(index==4){
   						this.menus[(index-1)].isActive =false;
   					}else{
   						this.menus[(index+1)].isActive =false;
   					}
   				}
 				return this.menus[index].isActive = !this.menus[index].isActive;
   			}*/
   		},
   		computed:{
            onRoutes(){
                return this.$route.path.replace('/','');
            }
        }
   }
</script>

<style scoped>
    .sidebar{
        display: block;
        position: absolute;
        width: 200px;
        left: 0;
        top: 66px;
        bottom:0;
        background: #324157;
       
    }
    .sidebar > ul {
        height:100%;
    }
	.sidebar ul>li{
		/*color:#ddd;line-height:50px;padding:0 20px;*/
	}
	.sidebar ul>li span{
		font-size:14px;
	}
	.sidebar ul>li .first-menu{
		color:#ddd;line-height:50px;padding:0 20px;
	}
	.sidebar ul>li .first-menu:hover{
		background:#48576a;cursor:pointer;
	}
	.sidebar ul>li  a{
		color:#fff;
	}
	/*二级菜单*/
	.second-menus{
		background:#1f2d3d;
	}
	.second-menus p{
		color:#fff;line-height:45px;font-size:14px;padding-left:40px;
	}
   .el-menu-item, .el-submenu__title{
       font-size:14px;
     
   }
   
    .material-icons {font-size:12px;}
</style>

