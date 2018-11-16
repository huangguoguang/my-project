<template>
    <div class="parent">
        我是父亲<br>
        <keep-alive>
            <component :is="currentView"></component>
        </keep-alive>
        <button @click="change">切换组件</button>
    </div>
</template>

<script>
import Son1 from "./Son1";
import Son2 from "./Son2";
export default {
  name: "parent",
  data() {
    return {
      currentView: "Son1",
      flag: true
    };
  },
  components: {
    Son1,
    Son2
  },
  methods: {
    change() {
      if (this.flag) {
        this.currentView = "Son2";
        this.flag = false;
      } else {
        this.currentView = "Son1";
        this.flag = true;
      }
    }
  }
};
</script>

<style scoped>
</style>


