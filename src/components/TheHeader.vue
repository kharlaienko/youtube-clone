<template>
	<header class="flex justify-between fixed z-30 w-full">
		<div class="lg:w-1/4 flex">
			<div class="flex items-center xl:w-64 xl:bg-white pl-4">
				<button class="mr-3 sm:ml-2 sm:mr-6 focus:outline-none">
					<base-icon iconName="menu"/>
				</button>
				<main-logo/>
			</div>
		</div>
		<div
			class="hidden sm:flex items-center justify-end p-2.5 pl-8 md:pl-12 md:px-8 flex-1 lg:px-0 lg:w-1/2 max-w-screen-md"
		>
			<the-search/>
			<the-voice-search/>
		</div>
		<div
			class="flex items-center justify-end lg:w-1/4 sm:space-x-3 p-2 sm:px-4"
		>
			<button class="sm:hidden p-2 focus:outline-none">
				<base-icon iconName="voice" class="w-5 h-5"/>
			</button>
			<button class="sm:hidden p-2 focus:outline-none">
				<base-icon iconName="search" class="w-5 h-5"/>
			</button>
			<button class="relative group p-2 focus:outline-none">
				<base-icon iconName="viewGrid" class="w-5 h-5"/>
		<!-- 		<drop-down-apps/> -->
			</button>
			<button class="relative group p-2 focus:outline-none">
				<base-icon iconName="threeDots" class="w-5 h-5"/>
			<!-- 	<drop-down-settings/> -->
			</button>
			<button-sign-in/>
		</div>
	</header>
</template>

<script>
import DropDownApps from './DropDownApps.vue'
import DropDownSettings from './DropDownSettings.vue'
import MainLogo from './MainLogo.vue'
import TheSearch from './TheSearch.vue'
import ButtonSignIn from './ButtonSignIn.vue'
import TheVoiceSearch from './TheVoiceSearch.vue'
import BaseIcon from './BaseIcon.vue'

export default {
	components:{
		DropDownApps,
		DropDownSettings,
		MainLogo,
		TheSearch,
		TheVoiceSearch,
		ButtonSignIn,
		BaseIcon
	}
}
</script>