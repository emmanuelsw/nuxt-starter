<template>
  <div>
    <el-row>
      <el-col :span="20" :offset="2">
        <el-card class="box-card">
          <div slot="header" >
            <span class="card-title">Latest Shows</span>
          </div>
          <el-row>
            <el-col :span="6" v-for="(o, index) in 2" :key="o" :offset="index > 0 ? 1 : 0">
              <el-card :body-style="{ padding: '0px' }">
                <img src="http://st.cdjapan.co.jp/pictures/l/05/36/TFXQ-78162.jpg" class="image">
                <div style="padding: 14px;">
                  <span>LEGEND - S - BAPTISM XX </span>
                  <div class="bottom clearfix">
                    <time class="time">2018-09-01 17:11</time>
                  </div>
                </div>
              </el-card>
            </el-col>
          </el-row>
        </el-card>
      </el-col>
    </el-row>
  </div>
</template>

<script>
export default {
  data() {
    return {}
  }
}
</script>

<style scoped>

.title {
  font-family: -apple-system, "Helvetica Neue", sans-serif;
  display: block;
  font-weight: 300;
  font-size: 40px;
  color: #35495e;
  letter-spacing: 1px;
}

.image {
  width: 100%;
}

.time {
  font-size: 13px;
  color: #999;
}

.card-title {
  font-family: 'Averia Serif Libre', cursive;
  font-size: 20px;
}

.links {
  padding-top: 15px;
}
</style>

