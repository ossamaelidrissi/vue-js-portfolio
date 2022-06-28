<script>
import projects from "../../data/projects";
import Project from "../Reusable/Project.vue";

export default {
    data: () => {
        return {
            projects
        };
    },
    components: { Project }
}
</script>

<template>
    <section className = "container mx-auto text-center flex flex-col items-center space-y-4 md:space-y-8 py-20" >
        <h1 className="text-2xl md:text-6xl tracking-tighter font-bold text-gray-800" >Projects Portfolio</h1>
        <p className = "text-lg md:text-xl text-gray-700" >Search projects by title or filter by category</p>
        <section className = "  md:space-x-3 md:w-3/4 flex flex-col md:flex-row space-y-3 md:space-y-0 items-center justify-between" >
            <section className = "flex items-center space-x-2" >
                <i className ='bx bx-search-alt-2 hidden md:flex text-3xl py-2 px-3 rounded-full bg-gray-100 ' />
                <input type="text" className = " py-2 md:py-3 px-3 md:px-4 border rounded-lg border-gray-200 shadow outline-none " placeholder="Search Projects" >
            </section>
            <select name="" id="" className = "border border-gray-200 shadow outline-none rounded-lg py-2 md:py-3 px-3 md:px-4" >
                <option value="">All Projects</option>
                <option value="">Web Application</option>
                <option value="">Mobile Application</option>
                <option value="">UI/UX Design</option>
                <option value="">Branding & Anim</option>
            </select>
        </section>

        <div className = "grid grid-cols-1 sm:grid-cols-2 mb-10 lg:grid-cols-3 gap-3 sm:gap-8 container mx-auto" >
            
            <Project v-for="project in projects"
                    :key="project.id"
                    :project="project" />
        </div>

        <router-link to = "/projects"  className = "text-base md:text-2xl py-2 px-4 mt-5 shadow-xl rounded bg-gray-800 text-white" >More Projects</router-link>
        
    </section>
</template>