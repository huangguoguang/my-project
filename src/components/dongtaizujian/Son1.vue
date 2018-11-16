<template>
    <div class="son1">
        {{msg}}
        <button @click="change">改变儿子1</button>
    </div>
</template>

<script>
export default {
  name: "son1",
  data() {
    return {
      msg: "我是儿子"
    };
  },
  methods: {
    change() {
      this.msg = "qqqqqqq";
    }
  }
};
</script>

<style scoped>
</style>


