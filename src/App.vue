<template>
	<the-header />
	<the-small-sidebar/>
	<the-sidebar/>
	<the-mobile-sidebar/>
	<the-categories/>
	<the-videos/>
</template>

<script>
import TheHeader from "./components/TheHeader.vue";
import TheSmallSidebar from "./components/TheSmallSidebar.vue";
import TheSidebar from "./components/TheSidebar.vue";
import TheMobileSidebar from "./components/TheMobileSidebar.vue";
import TheCategories from "./components/TheCategories.vue";
import TheVideos from "./components/TheVideos.vue";

export default {
	components: {
		TheHeader,
		TheSmallSidebar,
		TheSidebar,
		TheMobileSidebar,
		TheCategories,
		TheVideos
	},
};
</script>
