<template>
  <main>
    <!-- <img src="@/assets/images/arrow5.png" alt="arrow5" class="arrow5" />
    <img src="@/assets/images/arrow4.png" alt="arrow4" class="arrow4" />
    <img src="@/assets/images/arrow3.png" alt="arrow3" class="arrow3" />
    <img src="@/assets/images/arrow2.png" alt="arrow2" class="arrow2" />
    <img src="@/assets/images/arrow1.png" alt="arrow1" class="arrow1" /> -->
    <div class="mainTexts">
      <div class="text"> Hey <br>i'm partha <br> web developer
      <div class="homeButtons">
      <button-filled name="<AboutMe/>" />     
      <button-outline name="<ContactMe/>" />
      </div> 
      </div>
      <div class="mainLogo">
        <img src="@/assets/images/mainlogo.svg" alt="bigLogo" />
      </div>
    </div>
  </main>
</template>

<script>
import ButtonFilled from "@/components/buttons/ButtonFill.vue";
import ButtonOutline from "@/components/buttons/ButtonOutline.vue";
export default {
  name: "Home",
  components: {
    ButtonOutline,
    ButtonFilled,
  },
};
</script>

<style scoped>
main {
  width: 100vw;
  position: relative;
  min-height: calc(100vh - 70px);
  overflow: hidden;
  z-index: 50;
  margin-top: 70px;
  background-color: var(--primary-dark);
}

.mainTexts {
  display: flex;
  margin-top: 80px;
}
.text{
    width: 55%;
    z-index: 1;
    color: white;
    padding-left: 8vw;
    font-size: 80px;
    text-transform: capitalize;
}
.mainLogo{
    width: 45%;
    z-index: 1;
    padding-right: 1rem;
}
.mainLogo img{
    width: 100%;
}

.homeButtons{
    display: flex;
    justify-content: space-between;
    margin-top: 2rem;
    width: 50%;
}

 /* code for animatins */
/* main > img {
  position: absolute;
}
.arrow1 {
  right: 0vw;
  bottom: -90vh;
  width: 50%;
  z-index: 0;
  animation: moveup1 8s infinite linear;
  animation-delay: 3s;
}
.arrow2 {
  right: -5vw;
  bottom: -60vh;
  width: 20%;
  z-index: 2;
  animation: moveup2 8s infinite linear;
  animation-delay: 3s;
}
.arrow3 {
  left: 5vw;
  bottom: -60vh;
  width: 35%;
  z-index: 0;
  animation: moveup3 8s infinite linear;
  animation-delay: 3s;
}
.arrow4 {
  left: 10vw;
  bottom: -60vh;
  width: 10%;
  z-index: 2;
  animation: moveup4 8s infinite linear;
  animation-delay: 3s;
}
.arrow5 {
  right: 25vw;
  bottom: -60vh;
  width: 15%;
  z-index: 2;
  animation: moveup5 8s infinite linear;
  animation-delay: 3s;
}


@keyframes moveup1 {
  0% {
    transform: translateY(0);
  }
  30% {
    transform: translateY(-190vh);
  }
  100% {
    transform: translateY(-190vh);
  }
}
@keyframes moveup2 {
  0% {
    transform: translateY(0);
  }
  35% {
    transform: translateY(0vh);
  }
  65% {
    transform: translateY(-190vh);
  }
  100%{
    transform: translateY(-190vh);
  }
}
@keyframes moveup3 {
  0% {
    transform: translateY(0);
  }
  20% {
    transform: translateY(0vh);
  }
  50% {
    transform: translateY(-190vh);
  }
  100%{
    transform: translateY(-190vh);
  }
}
@keyframes moveup4 {
  0% {
    transform: translateY(0);
  }
  50% {
    transform: translateY(0vh);
  }
  80% {
    transform: translateY(-190vh);
  }
  100%{
    transform: translateY(-190vh);
  }
}
@keyframes moveup5 {
  0% {
    transform: translateY(0);
  }
  60% {
    transform: translateY(0vh);
  }
  90%{
    transform: translateY(-190vh);
  }
  100% {
    transform: translateY(-190vh);
  }
} */
</style>
