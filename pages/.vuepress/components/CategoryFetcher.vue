<template>
    <section>
        <ul>
            <li v-for="project in projects">
                <router-link :to="project.path">{{project.title}}</router-link>
            </li>
        </ul>
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
        let categoryName = this.$route.query.name;
        
        this.projects = this.$site.pages.filter(page=>{            
            return page.frontmatter.type == "project";
        }).filter(project=>{            
            return project.frontmatter.category==categoryName;
        })
    }
}
</script>