<template>
  <v-container class="fill-height">
    <v-responsive class="align-center text-center fill-height">
      <v-img height="120" src="@/assets/logo.svg"/>

      <h1 class="text-h2 font-weight-bold mt-5">RoboPPT</h1>

      <div class="text-h5 mt-2">汇聚全球优秀 PowerPoint 工程师</div>

      <div class="py-12"/>

      <v-row class="d-flex align-center justify-center">
        <v-col cols="auto">
          <v-menu>
            <template v-slot:activator="{ props }">
              <v-btn
                v-bind="props"
                color="warning"
                min-width="228"
                size="x-large"
                target="_blank"
                variant="flat"
              >
                <v-icon icon="mdi-file-powerpoint" size="large"/>
                机器人设计软件
              </v-btn>
            </template>
            <v-list>
              <v-list-item
                v-for="(item, index) in ppt_items"
                :key="index"
                :value="index"
                @click="openUrl(item.url)">
                <v-list-item-title>{{ item.title }}</v-list-item-title>
              </v-list-item>
            </v-list>
          </v-menu>
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
          <v-menu>
            <template v-slot:activator="{ props }">
              <v-btn
                v-bind="props"
                color="success"
                min-width="228"
                size="x-large"
                target="_blank"
                variant="flat"
              >
                <v-icon icon="mdi-cancel" size="large"/>
                不能水的比赛
              </v-btn>
            </template>
            <v-list>
              <v-list-item
                v-for="(item, index) in competition_items"
                :key="index"
                :value="index"
                @click="openUrl(item.url)">
                <v-list-item-title>{{ item.title }}</v-list-item-title>
              </v-list-item>
            </v-list>
          </v-menu>
        </v-col>
      </v-row>

      <div class="py-12"/>

      <v-row class="d-flex align-center justify-center">
        <v-col cols="auto">
          <div class="text-h6 text-red">
            tips: 申请加入QQ群请将申报书通过U盘或者移动硬盘寄送至大赛组委会。
          </div>
        </v-col>
      </v-row>
    </v-responsive>
  </v-container>
</template>

<script lang="ts">
import {defineComponent} from 'vue'

export default defineComponent({
  data() {
    return {
      ppt_items: [
        {title: "Microsoft 365", url: "https://www.microsoft.com/zh-cn/microsoft-365/powerpoint"},
        {title: "WPS Office", url: "https://www.wps.cn/"},
      ],
      competition_items: [
        {title: "RoboMaster", url: "https://www.robomaster.com/"},
        {title: "ROBOCON", url: "http://cnrobocon.net/"},
        {title: "ROBOTAC", url: "http://robotac.cn/"},
      ],
    }
  },
  methods: {
    openUrl(url: string) {
      window.open(url);
    }
  }
})
</script>
