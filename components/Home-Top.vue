<template>
  <el-container direction="vertical" class="home-top">
    <div class="color-line"></div>
    <div class="line background">
      <el-row class="title" justify="center">
          <el-col :span="14" :xs="24">
            <h1>Venez découvrir nos producteurs</h1>
          </el-col>
      </el-row>
      <img class="panneau" src="/images/entrant/panneau-500.png" alt="panneau">
    </div>
  </el-container>
</template>

<style lang="scss" scoped>
.home-top {
  z-index: 1;
}
.title {
  z-index: 10;
  display: flex;
  justify-content: center;
  .el-col,
  h1 {
    height: 100%;
  }
  h1 {
    line-height: 1.2;
    text-align: center;
    padding: 20px 40px;
    z-index: 20;
    background: rgba($green-d3, 0.5);
    &::after,
    &::before {
      margin: 30px auto;
      background-color: $white;
      height: 3px;
      width: 24vw;
      content: "";
      display: block;
    }
  }
}

@media (max-width: 450px) {
  .title {
    height: 100%;
    h1 {
      display: flex;
      flex-direction: column;
      justify-content: center;
    }
  }
}

.background {
  background-image: url("/static/images/entrant/credit-photo-Akim-Benbrahim.jpg");
  background-size: cover;
  background-position: center;
  height: calc(100vh - 55px);
}
.color-line {
  background: $green-d3;
}
.panneau {
  position: absolute;
  bottom: 0;
  left: 55px;
  height: 50%;
  opacity: 0.9;
  transform: rotate(3deg);
}
</style>
