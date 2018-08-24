<template>
  <panel title="新手特权" :class="$style.panel">
    <section :class="$style.content">
      <div :class="$style.item">
        <h4>下载App <span :class="$style.red">送888元礼包</span></h4>
        <p :class="$style.gray">新手专享</p>
        <img src="" alt="">
      </div>
      <div :class="$style.item">
        <ul>
          <li>
            <img src="" alt="">
            <h4 :class="$style.red">领128元新手礼包</h4>
            <p :class="$style.gray">立即开通</p>
          </li>
          <li>
            <img src="" alt="">
            <h4>打白条<span :class="$style.red">享免息</span></h4>
            <p :class="$style.gray">立即开通</p>
          </li>
        </ul>
      </div>
    </section>
  </panel>
</template>

<script>
import Panel from '../core/panel.vue'
export default {
  name: 'Novice',
  components: {
    Panel
  }
}
</script>

<style lang="scss" module>
@import '../../css/element.scss';
.panel {
  @include panel;
  >h4 {
    border-bottom: 1px solid #ddd;
  }
  .content {
    @include list(row);
    .item {
      width: 50%;
      box-sizing: border-box;
      &:first-child {
        padding: 32px 20px;
        border-right: 1px solid #ddd;
        img {
          width: 132px;
          height: 132px;
        }
      }
      h4 {
        font-size: 26px;
        line-height: 40px;
      }
      .red {
        color: #f00;
      }
      .gray {
        color: #999;
        font-size: 24px;
        text-align: center;
      }
      p {
        margin-top: 6px;
        font-size: 24px;
      }
      ul{
        width: 100%;
        height: 100%;
        li{
          width: 100%;
          height: 80px;
          padding: 32px 28px;
          box-sizing: border-box;
          &:first-child {
            border-bottom: 1px solid #ddd;
          }
          h4 {
            white-space: nowrap;
            text-overflow: ellipsis;
            overflow: hidden;
            text-align: left;
          }
          img{
            width: 80px;
            height: 80px;
            float: right;
          }
        }
        
      }
    }
  }
}
</style>
