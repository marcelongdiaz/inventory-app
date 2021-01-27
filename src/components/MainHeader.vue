<template>
	<div class="row cstm-container">
		<div class="col-md-2 header-1">
			<h1>{{ companyName }}</h1>
		</div>

		<div class="col-md-10 header-2">
			<div class="row">
				<div class="col-md-11">
					<input type="text" class="form-control" name="search" placeholder="Search for anything">
					
				</div>
				<div class="col-md-1">

					<span class="icon-cstm-notification"></span>
				</div>
			</div>
		</div>
	</div>
</template>
<script>
	export default{
		name: 'MainHeader',
		data(){
			return{
				companyName: 'Inventory'
			}
		}

	}
</script>
<style scoped>
.header-1{
	padding: 12px 0px;
	display: flex;
	justify-content: center;
	align-items: center;
	/* height: 100px; */
	/* width: 100%; */
	border: 2px dashed #f69c55;
}
.header-2{
	padding: 10px 30px
}
</style>