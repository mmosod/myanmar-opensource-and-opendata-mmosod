<template>
    <section>
        <h2>Categories</h2>
        <ul>
            <li v-for="category in categories">{{category}}</li>
        </ul>
    </section>
</template>

<script>

export default {
    data(){
        return {
            categories:[
                "Algorithms & Data Structures","Animation","Audio Processing","Build Tools","Compilers",
                "Data Science & ML","Data Sets","Development Tools","Electronics & Hardware",
                "Frameworks","Games","Graphics","Image","Mathematics",
                "Mobile","Networking","Open APIs","Operating Systems","Pdfs",
                "Security tools","Typography & Fonts","User Interface","Videos","Web",   
            ]
        }
    }
}
</script>

<style scoped>
    ul{
        list-style-type: none;
        padding: 0;
        display: flex;
        flex-wrap: wrap;
    }

    li{
        font-size: 0.8rem;
        padding: 5px 10px;
        background-color: #ddd;
        margin: 5px;
        border-radius: 10px;
    }

    li:hover{
        background-color: black;
        color:white;
        cursor: pointer;
    }
</style>