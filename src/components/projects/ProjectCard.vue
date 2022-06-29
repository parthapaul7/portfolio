<template>
  <div class="card">
    <div class="left">
      <div class="type">{{ project.type }}</div>
      <div class="name">{{ project.name }}</div>
      <div class="desc">
       {{project.description}} 
      </div>
      <div class="buttons">
        <ButtonFilled name="Visit Now" />
        <button-outline name="View Code" />
      </div>
    </div>
    <div class="right">
        <img src="@/assets/images/project.png" alt="project image">
    </div>
  </div>
</template>
<script>
import ButtonFilled from "@/components/buttons/ButtonFill.vue";
import ButtonOutline from "../buttons/ButtonOutline.vue";
export default {
  name: "projectCard",
  components: {
    ButtonFilled,
    ButtonOutline,
  },
  data() {
    return {
      project: {
        type: "Website",
        name: "Secure Blink",
        description: "This is front end project based on Vue.js and Vuex. Where i have i worked on basically in api intigrations and settuing up many tools for the functioning of the website",
        image: "",
        githubLink: "",
        siteLink: "",
      },
    };
  },
};
</script>
<style scoped>
.card {
  width: 60vw;
  max-width: 1000px;
  aspect-ratio: 2 / 1.1;
  margin: 0 auto;

  border: 2px yellow solid;
  border-radius: 70px;

  display: flex;
  justify-content: space-around;
}
.left {
  width: 50%;
  padding-left: 10%;
  padding-top: 6%;
}
.type {
  font-size: 24px;
}
.name {
  font-size: 40px;
  background-color: var(--primary-blue);
  width: fit-content;
  color: var(--primary-yellow);
  margin-top: 15px;
  border-radius: 10px;
}
.desc {
  margin: 50px 0;
  font-size: 18px;
}
.buttons{
    display: flex;
    justify-content: space-between;
    margin-right: 10%;
}
.right{
  width: 50%;
  margin: auto;
  padding-right: 20px;
}
.right img{
  width: 100%;
}
</style>
