<template>
    <div class="outer">
        <div>{{name}}</div>
    </div>
</template>
<script>
export default {
    name:"button-filled",
    props: {
        name: String
    },
    
}
</script>

<style scoped>
.outer{
    width: 150px;
    height: 40px;
    background-color: var(--primary-blue);
    color:white;

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
</style>