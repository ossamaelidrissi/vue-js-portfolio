<script>
import Projects from "../components/Shared/Projects.vue";
import Banner from "../components/Shared/Banner.vue";

export default {
	name: 'Home',
	components: {
		Banner,
		Projects
	},
};

</script>

<template>
    <section className = "container mx-auto " >
        <Banner />
        <Projects />
    </section>
</template>