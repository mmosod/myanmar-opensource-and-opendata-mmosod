<template>
    <section>
        <h2>Projects</h2>
        <article v-for="project in projects">
            {{project.title}}
            <div>
                <router-link :to="project.path">Go</router-link>
            </div>
        </article>
    </section>
</template>

<script>
export default {
    data(){
        return {
            projects:[]
        }
    },
    mounted(){
        let projects = this.$site.pages.filter(page=>{            
            return page.frontmatter.type == "project";
        })
        this.projects = projects;
    }
}
</script>

<style scoped>

</style>