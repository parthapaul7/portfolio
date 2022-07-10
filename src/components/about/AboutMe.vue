<template>
  <div class="main">
    <img src="@/assets/images/arrow5.png" alt="arrow5" class="arrow5" />
    <img src="@/assets/images/arrow4.png" alt="arrow4" class="arrow4" />
    <img src="@/assets/images/arrow3.png" alt="arrow3" class="arrow3" />
    <img src="@/assets/images/arrow2.png" alt="arrow2" class="arrow2" />
    <img src="@/assets/images/arrow1.png" alt="arrow1" class="arrow1" />
    <h1 class="heading">{{"<AboutMe />"}}</h1>
    <div class="underline"></div>
    <div class="content">
      <div class="left">
        <img src="@/assets/images/my-photo.png" alt="my image" />
      </div>
      <div class="right">
        <h2>{{ heading }}</h2>
        <p>{{ firstLine }}</p>
        <p>{{ secondLine }}</p>
        <div class="social">
          <h2>follow my work on</h2>
          <a>
            <svg
              fill="#FFFFFF"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 30 30"
              width="60px"
              height="60px"
            >
              <path
                d="M28,6.937c-0.957,0.425-1.985,0.711-3.064,0.84c1.102-0.66,1.947-1.705,2.345-2.951c-1.03,0.611-2.172,1.055-3.388,1.295 c-0.973-1.037-2.359-1.685-3.893-1.685c-2.946,0-5.334,2.389-5.334,5.334c0,0.418,0.048,0.826,0.138,1.215 c-4.433-0.222-8.363-2.346-10.995-5.574C3.351,6.199,3.088,7.115,3.088,8.094c0,1.85,0.941,3.483,2.372,4.439 c-0.874-0.028-1.697-0.268-2.416-0.667c0,0.023,0,0.044,0,0.067c0,2.585,1.838,4.741,4.279,5.23 c-0.447,0.122-0.919,0.187-1.406,0.187c-0.343,0-0.678-0.034-1.003-0.095c0.679,2.119,2.649,3.662,4.983,3.705 c-1.825,1.431-4.125,2.284-6.625,2.284c-0.43,0-0.855-0.025-1.273-0.075c2.361,1.513,5.164,2.396,8.177,2.396 c9.812,0,15.176-8.128,15.176-15.177c0-0.231-0.005-0.461-0.015-0.69C26.38,8.945,27.285,8.006,28,6.937z"
              />
            </svg>
          </a>
          <a>
            <svg
              fill="#FFFFFF"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 30 30"
              width="60px"
              height="60px"
            >
              <path
                d="M15,3C8.373,3,3,8.373,3,15c0,6.627,5.373,12,12,12s12-5.373,12-12C27,8.373,21.627,3,15,3z M10.496,8.403 c0.842,0,1.403,0.561,1.403,1.309c0,0.748-0.561,1.309-1.496,1.309C9.561,11.022,9,10.46,9,9.712C9,8.964,9.561,8.403,10.496,8.403z M12,20H9v-8h3V20z M22,20h-2.824v-4.372c0-1.209-0.753-1.488-1.035-1.488s-1.224,0.186-1.224,1.488c0,0.186,0,4.372,0,4.372H14v-8 h2.918v1.116C17.294,12.465,18.047,12,19.459,12C20.871,12,22,13.116,22,15.628V20z"
              />
            </svg>
          </a>
          <a>
            <svg
              fill="#FFFFFF"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 30 30"
              width="60px"
              height="60px"
            >
              <path
                d="M15,3C8.373,3,3,8.373,3,15c0,5.623,3.872,10.328,9.092,11.63C12.036,26.468,12,26.28,12,26.047v-2.051 c-0.487,0-1.303,0-1.508,0c-0.821,0-1.551-0.353-1.905-1.009c-0.393-0.729-0.461-1.844-1.435-2.526 c-0.289-0.227-0.069-0.486,0.264-0.451c0.615,0.174,1.125,0.596,1.605,1.222c0.478,0.627,0.703,0.769,1.596,0.769 c0.433,0,1.081-0.025,1.691-0.121c0.328-0.833,0.895-1.6,1.588-1.962c-3.996-0.411-5.903-2.399-5.903-5.098 c0-1.162,0.495-2.286,1.336-3.233C9.053,10.647,8.706,8.73,9.435,8c1.798,0,2.885,1.166,3.146,1.481C13.477,9.174,14.461,9,15.495,9 c1.036,0,2.024,0.174,2.922,0.483C18.675,9.17,19.763,8,21.565,8c0.732,0.731,0.381,2.656,0.102,3.594 c0.836,0.945,1.328,2.066,1.328,3.226c0,2.697-1.904,4.684-5.894,5.097C18.199,20.49,19,22.1,19,23.313v2.734 c0,0.104-0.023,0.179-0.035,0.268C23.641,24.676,27,20.236,27,15C27,8.373,21.627,3,15,3z"
              />
            </svg>
          </a>
          <a>
            <svg
              fill="#FFFFFF"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 48 48"
              width="60px"
              height="60px"
            >
              <path
                d="M 16.5 5 C 10.16639 5 5 10.16639 5 16.5 L 5 31.5 C 5 37.832757 10.166209 43 16.5 43 L 31.5 43 C 37.832938 43 43 37.832938 43 31.5 L 43 16.5 C 43 10.166209 37.832757 5 31.5 5 L 16.5 5 z M 16.5 8 L 31.5 8 C 36.211243 8 40 11.787791 40 16.5 L 40 31.5 C 40 36.211062 36.211062 40 31.5 40 L 16.5 40 C 11.787791 40 8 36.211243 8 31.5 L 8 16.5 C 8 11.78761 11.78761 8 16.5 8 z M 34 12 C 32.895 12 32 12.895 32 14 C 32 15.105 32.895 16 34 16 C 35.105 16 36 15.105 36 14 C 36 12.895 35.105 12 34 12 z M 24 14 C 18.495178 14 14 18.495178 14 24 C 14 29.504822 18.495178 34 24 34 C 29.504822 34 34 29.504822 34 24 C 34 18.495178 29.504822 14 24 14 z M 24 17 C 27.883178 17 31 20.116822 31 24 C 31 27.883178 27.883178 31 24 31 C 20.116822 31 17 27.883178 17 24 C 17 20.116822 20.116822 17 24 17 z"
              />
            </svg>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "about-me",
  data() {
    return {
      heading: "Hello Everyone",
      firstLine:
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco.",
      secondLine:
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
    };
  },
};
</script>
<style scoped>
.main {
  width: 100vw;
  min-height: 90vh;
  position: relative;
}
.heading {
  width: fit-content;
  margin: 0 auto;
  margin-top: 1rem;
  color: white;
  font-size: 36px;
}
.underline {
  width: 200px;
  margin: 0.25rem auto;
  margin-bottom: 5rem;
  height: 2px;
  background-color: white;
}
.content {
  display: flex;
}
.left {
  width: 35vw;
  padding-left: 10%;
}
.left img {
  width: 90%;
  margin: auto;
}
.right {
  width: 65vw;
  padding: 5%;
}
.right > p {
  font-size: 18px;
  line-height: 32px;
  margin: 50px 0;
}
.social h2 {
  text-transform: capitalize;
}
.social svg {
  width: 50px;
  margin: 0 8px;
  cursor:pointer ;
}

/* arrow animation */
.main > img {
  position: absolute;
}
.arrow1 {
  right: 0vw;
  bottom: -90vh;
  width: 50%;
  z-index: -1;
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
    opacity: 0;
  }
  1%{
    opacity: 100;
  }
  30% {
    transform: translateY(-200vh);
    opacity: 100;
  }
  31%{
    opacity: 0;
  }
  100% {
    transform: translateY(-200vh);
    opacity: 0;
  }
}
@keyframes moveup2 {
  0% {
    transform: translateY(0);
    opacity: 0;
  }
  35% {
    transform: translateY(0vh);
    opacity: 0;
  }
  36% {
    opacity: 100;
  }
  65% {
    transform: translateY(-190vh);
    opacity: 100;
  }
  66%{
    opacity: 0;
  }
  100% {
    transform: translateY(-190vh);
  }
}
@keyframes moveup3 {
  0% {
    transform: translateY(0);
    opacity: 0;
  }
  20% {
    transform: translateY(0vh);
    opacity: 0;
  }
  21% {
    opacity: 100;
  }
  50% {
    transform: translateY(-190vh);
    opacity: 100;
  }
  51%{
    opacity: 0;
  }
  100% {
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
  100% {
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
  90% {
    transform: translateY(-190vh);
  }
  100% {
    transform: translateY(-190vh);
  }
}
</style>
