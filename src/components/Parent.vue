<template>
    <div>
        <input type="text" v-model="num">
        <span v-bind:class="{isActive: flag}">这里是父亲</span><br>
        接收到儿子数据为:{{reciveMessage}}
        <Son @reciveMessage = "getMessage" :num = "getNum"></Son>
    </div>
</template>

<script>
import Son from "./Son";
export default {
  data() {
    return {
      flag: true,
      reciveMessage: "",
      num: 0
    };
  },
  computed:{
      getNum(){
          return this.num - 0;
      }
  },
  components: {
    Son
  },
  methods: {
    getMessage(data) {
      console.log(data);
      this.reciveMessage = data;
    }
  }
};
</script>

<style scoped>
.isActive {
  background-color: red;
  font-size: 20px;
}
</style>
