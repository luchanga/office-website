<template>
  <div class="layout-footer">
      <div class="container">
        <div class="footer-content">
            <div class="office-detail">
                <div class="logo">
                    <img src="../../assets/image/logo_white.png" alt="logo">
                </div>
                <ul class="list">
                    <li><i></i><span>152105****@qq.com</span></li>
                    <li><i></i><span>010-88886666</span></li>
                    <li><i></i><span>北京市昌平区回龙观镇黄平路19号院2号6层618-02</span></li>
                </ul>
            </div>
            <div class="about-detail footer-content-item">
                <h3>关于我们</h3>
                <ul class="list">
                    <li><a>联系我们</a></li>
                    <li><a>公司简介</a></li>
                    <li><a>公司资质</a></li>
                    <li><a>企业文化</a></li>
                    <li><a>人才招聘</a></li>
                </ul>
            </div>
            <div class="strategic-detail footer-content-item">
                <h3>战略合作</h3>
                <ul class="list">
                    <li><a>投资我们</a></li>
                    <li><a>加入我们</a></li>
                </ul>
            </div>
            <div class="solution-detail footer-content-item">
                <h3>解决方案</h3>
                <ul class="list">
                    <li><a>综合应急</a></li>
                    <li><a>风险管理</a></li>
                    <li><a>隐患管理</a></li>
                    <li><a>在线安全教育</a></li>
                </ul>
            </div>
        </div>
        <div class="info">
            ©2013-2020 北京华夏智邦科技有限公司 版权所有 京ICP备14060346号-1
        </div>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
    .layout-footer {
        width: 100%;
        height: 299px;
        background: #2C333D;
    }
    .container {
        padding: 45px 0 20px 0;
        height: 100%;
    }
    .footer-content {
        overflow: hidden;
        height: 200px;
        margin-bottom: 20px;
        .office-detail {
            width: 50%;
            float: left;
            .logo {
                margin-bottom: 20px;
                img {
                    width: 135px;
                    height: 36px;
                }
            }
        }
    }
    .footer-content-item {
        float: right;
        margin-left: 60px;
        h3 {
            margin-bottom: 20px;
            font-size: 16px;
            color: #E6E6E6;
        }
        .list {
            li {
                overflow: hidden;
                a {
                    font-size: 14px;
                    color: #6E7B8E; 
                }
            }
        }
    }
    .list {
        li {
            overflow: hidden;
            &:not(:first-of-type) {
                margin-top: 16px;
            }
            i {
                float: left;
                width: 14px;
                height: 14px;
                margin-right: 11px;
            }
            span {
                float: left;
                font-size: 14px;
                color: #6E7B8E;
            }
            a {
                font-size: 14px;
                color: #6E7B8E; 
            }
        }
    }
    .info {
        text-align: center;
        font-size: 12px;
        color: #6E7B8E;
    }
</style>