<template>
  <div>
    <Header></Header>

    <div class="block">
      <el-timeline>
        <el-timeline-item timestamp="2021/3/12" placement="top">
          <el-card>
            <h4>广东白云学院某学生买彩票中特等奖三百万，在此祝贺...</h4>
            <p>小明 提交于 2021/3/12 20:46</p>
          </el-card>
        </el-timeline-item>
        <el-timeline-item timestamp="2021/3/12" placement="top">
          <el-card>
            <h4>广东白云学院某学生买彩票中特等奖三百万，在此祝贺...</h4>
            <p>小明 提交于 2021/3/12 20:46</p>
          </el-card>
        </el-timeline-item>
        <el-timeline-item timestamp="2021/3/12" placement="top">
          <el-card>
            <h4>广东白云学院某学生买彩票中特等奖三百万，在此祝贺...</h4>
            <p>小明 提交于 2021/3/12 20:46</p>
          </el-card>
        </el-timeline-item>
        <el-timeline-item timestamp="2021/3/12" placement="top">
          <el-card>
            <h4>广东白云学院某学生买彩票中特等奖三百万，在此祝贺...</h4>
            <p>小明 提交于 2021/3/12 20:46</p>
          </el-card>
        </el-timeline-item>
        <el-timeline-item timestamp="2021/3/12" placement="top">
          <el-card>
            <h4>广东白云学院某学生买彩票中特等奖三百万，在此祝贺...</h4>
            <p>小明 提交于 2021/3/12 20:46</p>
          </el-card>
        </el-timeline-item>
      </el-timeline>

      <el-pagination class="m_page"
          background
          layout="prev, pager, next"
          :total="1000">
      </el-pagination>
    </div>
  </div>
</template>

<script>
import Header from "@/components/Header";
export default {
name: "test",
  components: {Header}
}
</script>

<style scoped>
.m_page{
  margin: 0 auto;
  text-align: center;
}
</style>