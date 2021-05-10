<template>
	<a
		href="#"
		:class="normalizedClasses"
		>{{ categoryName }}</a
	>
</template>

<script>
export default {
    props: {
        isActive: Boolean,
        categoryName: String
    },

    computed: {
        normalizedClasses(){
            const classes = ['px-3', 'py-1', 'transition', 'border', 'rounded-full']
            
            return this.isActive 
            ? [...classes, 'border-gray-700', 'bg-gray-600', 'hover:bg-gray-500', 'text-white']
            : [...classes, 'border-gray-300', 'bg-gray-100', 'hover:bg-gray-200']
        }
    }
}
</script>
