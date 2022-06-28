<script></script>
<template>
    <section className = "container mx-auto justify-around flex flex-col md:flex-row space-y-10 md:space-y-0 items-center mt-5 md:mt-0" >
        <section className = " flex flex-col items-center md:items-start space-y-4 text-center md:text-left" >
            <h1 className = " text-[1.8rem] md:text-[2.7rem] tracking-tighter	 font-bold text-gray-700" >HI , I'AM OSSAMA</h1>
            <p className = "text-xl md:text-2xl tracking-tighter	 text-gray-400 font-semibold" >A Full-Stack Developer & Design Enthusiast</p>
            <a href="/files/cv183.pdf" 
               download = "cv183.pdf" 
               className = "md:mr-auto px-3 md:px-5 my-10 text-gray-500 flex bg-gray-100 shadow-lg hover:bg-gray-800 hover:text-white duration-500 items-center py-2 space-x-3 border rounded-lg justify-center " >
                <section className = "md:text-2xl" >
                    <i class='bx bx-down-arrow-circle '></i>
                </section>
                <p className = "md:text-xl font-semibold " >Download CV</p>
            </a>
        </section>
        
        <img className = "w-3/4 md:w-1/2" src="https://vuejs-tailwindcss-portfolio.netlify.app/img/developer.d30886eb.svg" alt="banner picture">
        
    </section>
</template>