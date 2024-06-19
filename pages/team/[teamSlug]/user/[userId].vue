<script setup>
    const route = useRoute()
    const message = computed(() => `I am in a team of ${route.params.teamSlug} and my user id is ${route.params.userId}`)
</script>

<template>
    <div>
        {{ message }}
    </div>
</template>