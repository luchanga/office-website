<template>
  <div class="card">
      <div class="card-image">
          <img src="../../assets/image/card1.png" alt="">
      </div>
      <div class="card-text">
          <h4 class="card-title">中国石油应急管理系统</h4>
          <div class="card-description">值班管理系统是通过提高值班管理信息水平，积极促进健全值班管理工作体</div>
      </div>
      <div class="card-overlay">
          <div class="card-overlay-title">中国石油应急管理系统</div>
          <div class="card-overlay-description">值班管理系统是通过提高值班管理信息水平，积极促进健全值班管理工作体</div>
          <el-button round>查看详情</el-button>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped lang="scss">
    .card {
        width: 285px;
        height: 282px;
        overflow: hidden;
        cursor: pointer;
        position: relative;
        &:hover{
            .card-overlay {
                display: block;
                opacity: 1;
                transition: all 10s;
            }
            img {
                transform: scale(2.5);
                transition: all 500ms;
            }
        }
    }
    .card-overlay {
        opacity: 0;
        display: none;
        width: 100%;
        height: 100%;
        position: absolute;
        left: 0;
        top: 0;
        background: rgba(8,15,43,.8);
        padding: 0 20px;
        .el-button--medium.is-round {
            padding: 7px 22px;
            margin-top: 31px;
        }
    }
    .card-overlay-title {
        margin-top: 107px;
        color: #ffffff;
        font-size: 18px;
    }
    .card-overlay-description {
        margin-top: 15px;
        color: #ffffff;
        font-size: 14px;
        text-align: left;
    }
    .card-image {
        height: 180px;
        width: 100%;
        img {
            width: 100%;
            height: 100%;
        }
    }
    .card-text {
        height: 102px;
        width: 100%;
        background: #ffffff;
        padding: 16px 20px 20px 20px;
        h4 {
            font-size: 16px;
        }
        .card-description {
            margin-top: 15px;
            font-size: 14px;
            color: #999999;
            text-align: left;
            overflow : hidden;
            text-overflow: ellipsis;
            display: -webkit-box;
            -webkit-line-clamp: 2;
            -webkit-box-orient: vertical;
        }
    }
</style>