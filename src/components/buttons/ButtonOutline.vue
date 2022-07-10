<template>
    <div class="outer">
        <div>{{name}}</div>
    </div>
</template>
<script>
export default {
    name:"button-outline",
    props: {
        name: String
    },
    
}
</script>

<style scoped>
.outer{
    width: 150px;
    height: 40px;
    background-color: transparent;
    border: solid 1px var(--primary-blue);
    color: var(--primary-blue);

    border-radius: 8px;
    font-size: 18px;
    display: flex;
    align-items: center;

    cursor: pointer;
}
.outer div{
    height: fit-content;
    width: fit-content;
    margin: auto;
}

@media  screen and (max-width: 768px) {
    .outer{
        width: 120px;
        height: 30px;
        font-size: 12px;
    }
}
 
</style>