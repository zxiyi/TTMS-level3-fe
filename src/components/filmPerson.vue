<template>
	<div>
		<div style="width: 128px; height: 242px;margin-right: 18px; display: inline-block;" v-for="item in ggh">
			<!-- <div style="font-size: 16px; height: 20.8px; margin-bottom: 16px; text-align: left;">{{title}}</div> -->
			<el-image :src="item.img" style="width: 128px; height: 170px;"></el-image>
			<div style="margin-top: 8px;">{{item.name}}</div>
			<div style="color: #666666; font-size: 14px;margin-top: 5px;"><span v-if="actor!=''"></span>{{item.role}}</div>
		</div>
	</div>
</template>

<script>
  export default {
    data() {
      return {
        imgsrc: 'https://p1.meituan.net/moviemachine/750911af4331a708fd3be1b216d5e5c4134085.jpg@128w_170h_1e_1c',
        title: '导演',
        name:'罗永昌',
        actor:'李宝庭'
      }
    },
	props: {
	  ggh: Array
	},
  }
</script>

<style>
</style>
