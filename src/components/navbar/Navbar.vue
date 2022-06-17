<template>
    <nav>
        <div class="logoSm"><img src="@/assets/images/logo-sm.svg" alt="logo" lazy></div>
        <div class="navBtns">
            <NavButtons name="Home" :active="true"/>
            <NavButtons name="aboutMe" :active="false"/>
            <NavButtons name="Projects" :active="false"/>
            <NavButtons name="Contact" :active="false"/>
        </div>
    </nav>
</template>
<script>
import NavButtons from '@/components/navbar/NavButtons.vue';

export default {
    name: 'Navbar',
    components: {
        NavButtons
    }
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