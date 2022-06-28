<script>
    export default {
        name:"Project",
        props: ['project'],
        data() {
            return {
                //
            }
       }
    }
</script>

<template>
    <router-link to = "/projects/single-project" className = "flex flex-col items-center rounded-lg pb-5 mx-5 shadow-lg border" >
        <img className = "flex-grow object-cover md:h-3/4"  :src="project.img" :alt= "project.title">
        <h1 className = "text-2xl text-gray-800 pt-7 pb-2 font-semibold" >{{ project.title }}</h1>
        <h3 className = "text-lg font-semibold text-gray-600" >{{ project.category }}</h3>
    </router-link>
</template>