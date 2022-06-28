<template>
    
        
        <button @click="moveUp" class="text-3xl py-1 flex flex-col items-center space-y-4 w-full mx-auto bg-gray-50" >
            <i class='bx bxs-chevron-up' />
        </button>
        
    
</template>


<script>

    export default {
         methods:{
            moveUp(){
                window.scrollTo(
                    {
                        top:0,
                        behavior:'smooth'
                    }
                );
            }
        }
    }

</script>