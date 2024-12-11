<script setup>
    const route = useRoute()
    const {data} = useAsyncData(`/movies/${route.params.id}`,() => {
        return $fetch(`http://www.omdbapi.com/?apikey=a2e4475f&i=${route.params.id}`)
    }, {
        pick: ['Plot','Title'],
        // transform(data){
        //     return {
        //         Plot: data.Plot,
        //         Title: data.Title
        //     }
            
        // }
    })
    
</script>


<template>
    <div>
        <pre>{{ data }}</pre>
    </div>
</template>