<template>
  <div class="main_wrapper">
 
    <transition name="fade">
      <router-view></router-view>
    </transition>
  </div>
</template>

<script>
import SpiderSolitaire from "./views/Spider.vue";
import KlondikeSolitaire from "./views/Klondike.vue";

export default {
  name: "mainTable",
  components: { SpiderSolitaire, KlondikeSolitaire },
  data: function() {
    return {
      chosen: false
    };
  }
};
</script>
<style >
@media screen and (max-width: 800px) {
  .github-fork-ribbon {
    display: none;
  }
}
</style>

