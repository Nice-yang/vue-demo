
<!--菜单-->
<template>
	<div>
		<v-pageTitle vtitle="TodoList"></v-pageTitle>
		<TodoList></TodoList>
	</div>
</template>
<script	>
	import vPageTitle from '../common/pageTitle'
	import TodoList from '../todoList/TodoList';
	export default {
		components:{
			vPageTitle,TodoList
		}
	}
</script>