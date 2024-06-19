<script setup>
    const route = useRoute()
    const message = computed(() => `The dynamic page with route params ${route.params.id}`)
</script>

<template>
    <div>
        {{message}}
    </div>
</template>