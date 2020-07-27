<template>
  <div class="panelTitle">
      <div class="title">
          <h2 class="title-bg">
              {{aliasName}}
          </h2>
          <h3>{{name}}</h3>
      </div>
  </div>
</template>

<script>
export default {
    props: {
        name: String,
        aliasName: String
    }
}
</script>

<style scoped lang="scss">
@import '@/assets/styles/variables.scss';
    .panelTitle {
        width: 100%;
        height: 70px;
        text-align: center;
        margin-bottom: 19px;
        .title {
            height: 100%;
            position: relative;
            .title-bg {
                display: inline-block;
                position: absolute;
                left: 50%;
                transform: translateX(-50%);
                font-weight: normal;
                font-size:80px;
                color:#F0F0F0;
                top: -15px;
            }
            h3 {
                display: inline-block;
                font-size: 30px;
                color: $black;
                position: absolute;
                left: 50%;
                transform: translateX(-50%);
                top: 16px;
                &:after {
                    content: '';
                    height: 3px;
                    display: block;
                    background: #1A96D5;
                    width: 80%;
                    margin: 20px auto 0 auto;
                }
            }
        }
    }
</style>