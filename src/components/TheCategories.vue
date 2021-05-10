<template>
    	<section
		class="pt-14 md:pl-24 xl:pl-64 w-full fixed bg-white bg-opacity-95 z-10"
	>
		<div class="border-t border-b px-4 max-w-screen-2xl m-auto">
			<div
				class="py-3 flex space-x-3 overflow-auto text-sm whitespace-nowrap"
			>
				<category-item v-for="name in categoriesNames" :key="name" :categoryName="name" :isActive="name === 'All'"/>
			</div>
		</div>
	</section>
</template>

<script>
import CategoryItem from './CategoryItem.vue'

export default {
	components: {
		CategoryItem,
	},

	data(){
		return{
			categoriesNames: [
				'All',
				'Trucks',
				'Tools',
				'Machines',
				'Engines',
				'Snow',
				'Ships',
				'Roads',
				'Tanks',
				'Building',
				'Mars',
				'Woodworking',
				'Tractors',
				'Songs',
				'TV Show',
				'Football',
				'Planes',
				'Live',
				'Streets',
				'Math',
				'Programming',
			]
		}
	}
}
</script>