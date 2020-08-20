<template>
    <div>
        <h1 class="subtitle">About</h1>
		<div class="about">
			<p class="text">Hi! I'm Aoshi.<br>I’ve always liked that I find that I’ve not knew thing.
If I’m into a thing at even once, It isn’t easy to stop the thing.</p>
			<p>~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</p>
			<div class="introduce">
				<div class="name">
					<h3>Name:</h3>
					<p>Aoshi Suzuki</p>
				</div>
				<div class="name">
					<h3>School:</h3>
					<p>The University of Aizu</p>
				</div>
				<h3>Language:</h3>
				<div class="lang">
					<img src="../components/images/python.svg" alt="logo" class="lang-image" width="3%">
					<p>Python</p>
				</div>
				<div class="lang">
					<img src="../components/images/R.svg" alt="logo" class="lang-image">
					<p>R</p>
				</div>
				<div class="lang">
					<img src="../components/images/c++.svg" alt="logo" class="lang-image">
					<p>C++(Studying)</p>
				</div>
				<div class="lang">
					<img src="../components/images/julia.svg" alt="logo" class="lang-image">
					<p>Julia(will study)</p>
				</div>
			</div>
		</div>
    </div>
</template>


<style>
@import url('https://fonts.googleapis.com/css2?family=Antic+Slab&display=swap');
.about{
	display: flex;
	flex-direction: column;
	padding-left: 5%;
	padding-right: 5%;
	font-family: 'Antic Slab', serif;
}
.subtitle{
	
}
.text{
	
}

.lang{
	display: flex;
	flex-direction: row;
	align-items: center;
}
.name{
	display: flex;
	flex-direction: row;
	align-items: baseline;
	margin-right: 10px;
}
.lang-image{
	margin-right: 7px;
	width:6%;
}
.per_intro{
	float: left;
}
</style>