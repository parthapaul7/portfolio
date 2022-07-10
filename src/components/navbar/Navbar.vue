<template>
    <nav>
        <div class="logoSm"><img src="@/assets/images/logo-sm.svg" alt="logo" lazy></div>
        <div class="navBtns">
            <NavButtons name="Home"  @scroll="scrollTo" :position="scrollPositions[0]"/>
            <NavButtons name="aboutMe"  @scroll="scrollTo" :position="scrollPositions[1]"/>
            <NavButtons name="Projects" @scroll="scrollTo" :position="scrollPositions[2]"/>
            <NavButtons name="Contact" @scroll="scrollTo" :position="scrollPositions[3]"/>
        </div>
    </nav>
</template>
<script>
import NavButtons from '@/components/navbar/NavButtons.vue';

export default {
    name: 'Navbar',
    components: {
        NavButtons
    },
    data() {
        return {
            scrollPositions: [
                {
                    name: 'Home',
                    x: 0,
                    y: 0,
                    active: true
                },
                {
                    name: 'aboutMe',
                    x: 0,
                    y:700,
                    active: false,
                },
                {
                    name: 'Projects',
                    x: 0,
                    y: 1500,
                    active: false,

                },
                {
                    name: 'Contact',
                    x: 0,
                    y: 0,
                    active: false,
                }
            ],
        }
    },
    methods: {
        scrollTo(x,y,name) {
            this.scrollPositions.forEach((item,index)=>{
                if(item.name==name){
                    this.scrollPositions[index].active=true;
                }else{
                    this.scrollPositions[index].active=false;
                }
            });
            console.log("name",name,this.scrollPositions);
            window.scrollTo(x, y);
        }
    },
}
</script>
<style scoped>
   nav{
    width: 100%;
    height: 70px;
    display: flex;
    justify-content: space-between;
    align-content: center;
    background-color: var(--nav-blue);
    color: white;

    position: fixed;
    top: 0;
    z-index: 100;
   } 
   .navBtns{
    width: 40%;
    margin-left: auto;
    display: flex;
    justify-content: space-evenly;
    align-items: center;
   }
   .navBtns > div{
    height: fit-content;
   }
   .logoSm{
    margin-left: 1rem;
   }
</style>