<template>
  <div>
    <div class="pageTitle">猫眼电影</div>
    <ul class="topNav">
      <li :class="[showHot == 1?'active':'']" @click = 'showHot = 1'>正在热映</li>
      <li :class="[showHot == 0?'active':'']" @click="showHot = 0 ">即将上映</li>
    </ul>
  </div>
</template>

<script>
import hoting from '@/components/hoting'
import comming from '@/components/cinnubg'
export default {
  name: "index",
  comments:{
    hoting,comming
  },
  data() {
    return {
      showHot:1
    };
  }
};
</script>

<style scoped>
color:rgb(229,72,71);
border-bottom:2px solid rgb(229,72,71);
</style>
