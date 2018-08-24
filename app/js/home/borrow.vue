<template>
  <Panel title="极速借贷" :class="$style.panel">
    <select :class="$style.content">
      <router-link :to="{name:'home'}">
        <img src="https://img12.360buyimg.com/jrpmobile/jfs/t22684/335/2434116613/75683/d2d0f2fc/5b7e91e6Ne96a57a1.jpg?width=750&height=320">
      </router-link>
    </select>
  </Panel>
</template>

<script>
import Panel from '../core/panel.vue';
export default {
  components: {
    Panel
  }
}
</script>

<style lang="scss" module>
@import '../../css/element.scss';
.panel {
  @include panel;
  .content {
    padding-bottom: 40px;
    img{
      display: block;
      width: 300px;
      height: 700px;
    }
  }
}
</style>

