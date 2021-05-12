<template>
	<div class="flex w-full h-full">
        <the-search-input/>
        <the-search-button/>
	</div>
</template>

<script>
import TheSearchInput from './TheSearchInput.vue'
import TheSearchButton from './TheSearchButton.vue'


export default {
    components: {
        TheSearchInput,
        TheSearchButton
    }
}
</script>