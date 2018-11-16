<template>
    <div>
        我是父亲
        <Son>
            <p slot="s1">我是插槽1</p>
            <p slot="s2" slot-scope="props">我是插槽2 + {{props.text}}</p>
            <hr>
            <p>我是插槽1</p>
            <p>我是插槽2</p>
        </Son>
    </div>
</template>


<script>
import Son from "./Son";
export default {
  name: "parent",
  data() {
    return {};
  },
  components: {
    Son
  }
};
</script>


<style scoped>
</style>
