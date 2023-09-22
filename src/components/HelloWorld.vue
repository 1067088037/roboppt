<template>
  <v-container class="fill-height">
    <v-responsive class="align-center text-center fill-height">
      <v-img height="120" src="@/assets/logo.svg"/>

      <h1 class="text-h2 font-weight-bold mt-5">RoboPPT</h1>

      <div class="text-h5 mt-2">汇聚全球优秀 PowerPoint 工程师</div>

      <div class="py-12"/>

      <v-row class="d-flex align-center justify-center">
        <v-col cols="auto">
          <v-btn
            color="warning"
            href="https://www.microsoft.com/zh-cn/microsoft-365/powerpoint"
            min-width="228"
            size="x-large"
            target="_blank"
            variant="outlined"
          >
            <v-icon icon="mdi-file-powerpoint" size="large"/>
            机器人设计软件
          </v-btn>
        </v-col>

        <v-col cols="auto">
          <v-btn
            color="primary"
            href="https://www.zhihu.com/question/623044430"
            min-width="228"
            size="x-large"
            target="_blank"
            variant="flat"
          >
            <v-icon icon="mdi-forum" size="large"/>
            加入讨论
          </v-btn>
        </v-col>

        <v-col cols="auto">
          <v-btn
            color="primary"
            href="http://wx.youngcommunist.com/#/microtabs/microstationdetail?activityid=HD-2309160037"
            min-width="228"
            size="x-large"
            target="_blank"
            variant="outlined"
          >
            <v-icon icon="mdi-bulletin-board" size="large"/>
            大赛通知
          </v-btn>
        </v-col>
      </v-row>

      <div class="py-12"/>

      <v-row class="d-flex align-center justify-center">
        <v-col cols="auto">
          <div class="text-h6 text-red">
            tips: 申请加入QQ群请将申报书通过U盘或者移动硬盘寄送至大赛组委会秘书处。
          </div>
        </v-col>
      </v-row>
    </v-responsive>
  </v-container>
</template>

<script lang="ts" setup>
//
</script>
