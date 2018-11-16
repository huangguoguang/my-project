<template>
    <div class="son">
        我是儿子
        <div>
            <slot name="s1"></slot>
            <slot name="s2" text="我是s2"></slot>
        </div>
    </div>
</template>


<script>
export default {
    name: "son",
    data(){
        return{

        }
    }
}
</script>


<style scoped>
    .son{
        background-color: red;
        width: 800px;
        height: 300px;
    }
</style>
