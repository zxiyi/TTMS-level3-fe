<template>
  <div class="clpn">
	<!-- 	style="height: 800px;" -->
    <el-tabs :tab-position="tabPosition" v-model="activeName" style="min-height:300px">
      <el-tab-pane label="个人信息" name="second">
        <u-pifn></u-pifn>
      </el-tab-pane>
      <el-tab-pane label="订单信息" name="first">
        <u-order></u-order>
      </el-tab-pane>
    </el-tabs>
  </div>
</template>

<script>
  import uPifn from './UserPifn.vue'
  import uOrder from './UserOrder.vue'
  export default {
    data() {
      return {
        tabPosition: 'left',
        activeName: 'first',
      };

    },
    components: {
      uPifn,
      uOrder,
    },
    methods: {
      asd(name) {
        console.log(name);
      }
    },
  }
</script>

<style scoped>
  .clpn {
    margin: 0 auto;
    width: 1050px;
  }
</style>
