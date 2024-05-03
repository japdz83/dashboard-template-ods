<script setup>
import BannerIntro from '@/components/BannerIntro.vue';
import StatisticsCard from '../components/Cards/StatisticsCard.vue'
</script>

<template>
	<BannerIntro />
	<div class="content px-3 py-4">
		<div class="container-fluid">
			<div class="mb-3 d-flex justify-content-center w-auto">
				<div class="flotar w-100 d-flex justify-content-center">
					<div class="row justify-content-between ">
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
	position: absolute;

	top: -4rem;
	padding: 0 4rem 0 0;
}
</style>
