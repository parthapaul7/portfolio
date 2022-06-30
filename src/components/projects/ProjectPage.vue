<template>
    <div class="main">
        <h1 class="heading">{{"<Projects/>"}}</h1>
        <div class="underline"></div>
        <project-card/>
    </div>
</template>
<script>
import ProjectCard from './ProjectCard.vue'
export default {
  components: { ProjectCard },
    name:"ProjectPage",
    data(){
        return{
            project: {
                name: "",
                description: "",
                image: "",
                link: "",
                tags: [],
                date: "",        
            }
        }
    }
}
</script>
<style scoped>
.main{
    width: 100vw;
    min-height: 90vh;
}
.heading{
    width: fit-content;
    margin:5rem auto;
    margin-bottom: 0;
    color: white;
    font-size: 36px;
}
.underline{
    width: 200px;
    margin:0.25rem auto;
    margin-bottom: 5rem;
    height: 2px;
    background-color: white;
}
</style>