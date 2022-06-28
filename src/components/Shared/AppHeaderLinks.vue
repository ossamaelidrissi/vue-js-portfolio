<script>

    export default {
        props: [ 'showModal ' , 'isOpen' ],
        data() {
            return {
                theme : ''
            }
        },
        methods: {
            updateTheme(theme) {
                this.theme = theme
            }
        }
    }
</script>

<template>
    <div className = "m-0 sm:ml-4 mt-5 sm:mt-3 sm:flex p-5 sm:p-0 justify-center items-center shadow-lg sm:shadow-none">
        <router-link 
             to = "/projects"
             className = "" 
             >
            Projects
        </router-link>
        <router-link 
             to = "/projects"
             className = "" 
             >
            Projects
        </router-link>
        <router-link 
             to = "/projects"
             className = "" 
             >
            Projects
        </router-link>
    </div>

</template>