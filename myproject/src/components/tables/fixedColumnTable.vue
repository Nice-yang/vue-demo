<template>
	<el-table :data="tableData" style="width:100%" border stripe>
		<el-table-column fixed prop="id" label="ID"></el-table-column>
		<el-table-column prop="username" label="autor"></el-table-column>
		<el-table-column prop="age" label="age"></el-table-column>
		<el-table-column prop="ability" label="ability"></el-table-column>
		<el-table-column prop="value" label="value"></el-table-column>
		
	</el-table>
</template>
<script>
	export default{
		data(){
			return {
				tableData:[
					{
						id:1,
						username:'yhj',
						age:12,
						ability:'websiet',
						value:'90%'
					},
						{
						id:2,
						username:'yhj',
						age:12,
						ability:'websiet',
						value:'90%'
					},
						{
						id:3,
						username:'yhj',
						age:12,
						ability:'websiet',
						value:'90%'
					},
						{
						id:4,
						username:'yhj',
						age:12,
						ability:'websiet',
						value:'90%'
					},
						{
						id:5,
						username:'yhj',
						age:12,
						ability:'websiet',
						value:'90%'
					},
						{
						id:6,
						username:'yhj',
						age:12,
						ability:'websiet',
						value:'90%'
					},
						{
						id:7,
						username:'yhj',
						age:12,
						ability:'websiet',
						value:'90%'
					},
						{
						id:8,
						username:'yhj',
						age:12,
						ability:'websiet',
						value:'90%'
					},
				]
			}
		}
	}
</script>
<style scoped>
    
</style>
