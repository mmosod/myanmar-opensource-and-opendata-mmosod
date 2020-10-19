<template>
    <section>
        <h3>Title - {{$page.title}}</h3>
        <p>Creator - {{$page.frontmatter.creator}}</p>  
        <p>Soruce - <a :href="$page.frontmatter.link" target="_b">{{$page.frontmatter.link}}</a></p> 
    </section>    
</template>

<script>
export default {
    
}
</script>

<style scoped>

</style>