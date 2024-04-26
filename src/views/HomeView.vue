<script setup>
import BannerIntro from '../components/BannerIntro.vue'
import StatisticsCard from '../components/Cards/StatisticsCard.vue'
</script>

<template>
	<BannerIntro />
	<div class="content px-3 py-4">
		<div class="container-fluid">
			<div class="mb-3">
				<div class="flotar">
					<div class="row">
						<div class="col-lg-2 col-md-6 col-12">
							<StatisticsCard />
						</div>

						<div class="col-lg-2 col-md-6 col-12">
							<StatisticsCard />
						</div>

						<div class="col-lg-2 col-md-6 col-12">
							<StatisticsCard />
						</div>

						<div class="col-lg-2 col-md-6 col-12">
							<StatisticsCard />
						</div>

						<div class="col-lg-2 col-md-6 col-12">
							<StatisticsCard />
						</div>

						<div class="col-lg-2 col-md-6 col-12">
							<StatisticsCard />
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>

<style scoped>
.content{
	position: relative;
}

.flotar{
	width: 100%;
	position: absolute;
	top: -4rem;
	padding: 0 4rem 0 0;
}
</style>
