<template>
    <div class="btn" @click="makeActive">
       <div :class="['btnName' , this.position.active && 'highlight']">{{"<"}}{{name}}{{"/>"}}</div> 
       <div  :class="['underline', !this.position.active&& 'invisible animate-underline']"></div>
    </div>  
</template>

<script>
export default {
   name: 'NavButtons', 
   emits: ['scroll'],
   props: {
      name:String,
      position:Object,
      
   },
   data(){
      return {
      }
   },
   methods:{
      makeActive(){
        this.$emit('scroll',this.position.x,this.position.y,this.position.name);
        // this.isActive= true;
      }
   }
}
</script>
<style scoped>
    .underline{
        width: 90%;
        height: 2px;
        background-color: white;
        margin: 1px auto;
    }
    .invisible{
        width: 0;
    }
    .btn{
        cursor: pointer;
        font-size: 16px;
        font-weight: 300;
    }
    .btnName{
        text-transform: capitalize;
    }
    
    .highlight{
        font-size: 18px;
        font-weight: 400;
    }
    .btn:hover{
        font-weight: 400;
    }
    .btn:hover .animate-underline{
        animation: animate-underline 1s linear; 
    }
    @keyframes animate-underline{
        0%{
            width: 0%;
        }
        50%{
            width: 90%;
        }
        100%{
            width: 0%;
        }   
    }
</style>
