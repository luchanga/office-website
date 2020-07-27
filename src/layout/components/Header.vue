<template>
    <div class="layout-header">
        <nav class="nav container">
            <div class="logo">
                <router-link to="/">
                    <img src="../../assets/image/logo.png" alt="logo">
                </router-link>
            </div>
            <div class="nav-menu">
                <el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal">
                    <el-menu-item v-for="(routeObj, index) in mainRoutes" :index="index.toString()" :key="routeObj.name">
                        <router-link :to="routeObj.path">{{routeObj.name}}</router-link>
                    </el-menu-item>
                </el-menu>
            </div>
        </nav>
    </div>
</template>

<script>
import { mainRoutes } from '@/router';
export default {
    name: 'app-header',
    data() {
      return {
        activeIndex: '0',
        mainRoutes: mainRoutes
      };
    },
    mounted() {
    }
}
</script>

<style lang="scss" scoped>
@import '@/assets/styles/variables.scss';
@import '@/assets/styles/mixin.scss';
    .layout-header {
        width: 100%;
        height: 60px;
        background: #ffffff;
    }
    .nav {
        height: 100%;
        padding: 12px 0;
        overflow: hidden;
    }
    .logo {
        float: left;
        img {
            width: 135px;
            height: 36px;
        }
    }
    .nav-menu {
        float: right;
        .el-menu--horizontal {
            border-bottom: 0;
            & >.el-menu-item {
                height: 36px;
                line-height: 36px;
                margin-left: 20px;
                padding: 0;
                color: $black;
                font-size: 16px;
                &:hover {
                    color: #1A96D5;
                }
                &.is-active {
                    border-bottom: 2px solid #1A96D5;
                    color: #1A96D5;
                    font-weight: bold;
                }
            }
        }
    }
</style>