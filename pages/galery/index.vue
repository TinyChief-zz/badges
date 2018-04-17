<template>
	<section class="galery-page">
		<div class="section-title">
			<h1>
				Галерея значков
			</h1>
		</div>
		<div class="section-content">
			<div class="filter">
				<h2>Тут будет фильтр</h2>
			</div>
			<Badges></Badges>
		</div>
	</section>
</template>

<script>
import Badges from '@/pages/galery/components/Badges';
export default {
	components: {
		Badges
	}
}
</script>

<style scoped>
.filter{
	height: 100px;
	background: #ccc;
	margin-bottom: 15px;
}


</style>
