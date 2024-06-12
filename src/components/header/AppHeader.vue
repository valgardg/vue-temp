<template>
	<nav class="navbar sticky-top navbar-expand-lg header-div">
		<div class="container-fluid d-flex justify-content-between">
			<div class="col-2">
				<img src="@/assets/images/iceland-mountains.png" class="header-logo" />
			</div>
			<div class="col-2 d-flex justify-content-end">
				<button class="btn generic-header-button">Button</button>
			</div>
		</div>
	</nav>
</template>

<style scoped>
.header-div {
	margin-top: 0px;
	padding: 18px 10px;
	background-color: #bfeadd;
	border: 0px;
	border-bottom: 2px;
	border-style: solid;
	border-color: rgb(0, 135, 97);
}
.header-logo {
	width: 140px;
	height: 40px;
	margin-left: 4rem;
}
.generic-header-button {
	margin-right: 4rem;
	color: white;
	background-color: rgb(5, 183, 121);
	font-weight: 600;
}
</style>