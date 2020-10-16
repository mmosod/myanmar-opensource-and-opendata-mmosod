<template>
    <main>
        <h2>Projects</h2>
        <section class="container">
            <article class="card" v-for="project in projects">
                <h3>{{project.title}}</h3>
                <span>{{project.frontmatter.category}}</span>
                <h4>Creator - <em>{{project.frontmatter.creator}}</em></h4>
                <div class="goto-button">
                    <router-link :to="project.path">အသေးစိတ်ကြည့်ရန်</router-link>
                </div>
            </article>
        </section>
    </main>
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
        this.projects = projects.reverse();
    }
}
</script>

<style scoped>
    .container{
        display:flex;
        margin-bottom: 16px;
        flex-wrap: wrap;
        justify-content: space-around;
    }

    .card{
        flex-basis: 240px;
        padding: 0 16px;
        margin-bottom: 16px;
        border-radius: 8px;
        box-shadow: 0 2px 2px 0 rgba(0,0,0,0.14), 0 3px 1px -2px rgba(0,0,0,0.12), 0 1px 5px 0 rgba(0,0,0,0.20);
    }

    .card h3{
        margin: 4px 0;
    }

    .card span{
        display: inline-block;
        background-color: rgba(0, 0, 0, 0.7);
        color:white;
        padding: 4px 8px;
        font-size: 8px;
        border-radius: 16px;
    }
    .card h4{
        margin: 8px 0;
    }

    .goto-button{
        border-top:1px solid darkgray;
        padding: 8px 0;
    }

    .goto-button a{
        text-transform: uppercase;
        font-size: 12px;
    }

    @media (max-width:560px){
        .card{
            flex-basis: 360px;
        }
    }
</style>