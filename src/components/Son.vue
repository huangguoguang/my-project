<template>
    <div>
        这里是儿子
        <button @click="sendMessage">向父亲传递消息</button>
        父亲传过来的值为{{num}}
    </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  props:{
      num:{
          type: Number,
          default: 5
      }
  },
  computed:{
      addNum(){
          return this.num * 5
      }
  },
  methods: {
    sendMessage(event) {
        console.log(event)
        this.$emit("reciveMessage", this.addNum);
    }
  }
};
</script>

<style scoped>
</style>
