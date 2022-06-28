<script>

    export default {
        name:"Header",
        data() {
            return {
                theme : 'light'
            }
        },
        methods: {
           toggleTheme() {
            	const newTheme = this.theme === 'light' ? 'dark' : 'light';
                localStorage.setItem("theme",newTheme)

           }
        }
    }
</script>
<template>
    <header className = " py-5 flex items-center justify-around" >
        <router-link to = "/">
            <img className = "h-16 md:h-28 cursor-pointer"  alt="Vue logo" src="../../assets/images/logo.png" />
        </router-link>
        <nav className = " hidden md:flex items-center space-x-12 text-gray-700 " >
            <router-link className = "text-xl font-semibold cursor-pointer hover:text-gray-80"  to = "/projects" >Projects</router-link> 
            <router-link className = "text-xl font-semibold cursor-pointer hover:text-gray-80"  to = "/about" >About Me</router-link> 
            <router-link className = "text-xl font-semibold cursor-pointer hover:text-gray-80"  to = "/contact" >Contact</router-link> 
        </nav>
        <section className = "flex items-center space-x-5 " >
            <button className = "bg-gray-600 hidden md:flex hover:bg-gray-800 duration-300 text-white rounded-lg px-4 py-3 font-semibold text-xl" >Hire Me</button>
            <div @click ="toggleTheme" className = "text-2xl" >
                <i className='bx bx-moon  bg-gray-100 cursor-pointer p-3 rounded-xl' />
            </div>
            <div  className = "text-2xl md:hidden" >
                <i className='bx bx-menu  bg-gray-100 cursor-pointer p-3 rounded-xl' />
            </div>

        </section>
    </header>
</template>