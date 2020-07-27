<template>
    <div>
            <carousel></carousel>
            <div class="case">
                <div class="container">
                    <div class="content">
                        <panelTitle name="案例中心" aliasName="Case"/>
                        <span class="description">我们基于用户的需求主导产品研发，提供丰富、安全、易用、灵活的服务。</span>
                        <div class="card-list">
                            <card/>
                            <card/>
                            <card/>
                            <card/>
                        </div>
                    </div>
                    <div class="content">
                        <panelTitle  name="解决方案" aliasName="SOLUTIONS"/>
                        <span class="description">公司产品广泛应用于综合应急、风险管理、隐患管理、在线安全教育、养老服务、开发平台、生产集成平台等领域。</span>
                    </div>
                </div>
            </div>
    </div>
</template>

<script>
import Carousel from '@/components/carousel'
import PanelTitle from '@/components/panelTitle'
import Card from '@/components/card'
export default {
    components: {
        Carousel,
        PanelTitle,
        Card
    }
}
</script>

<style lang="scss">
@import '@/assets/styles/variables.scss';
    .case {
        background: #f5f5f5;
        text-align: center;
        padding: 50px 0 40px 0;
        .description {
            padding-top: 19px;
            color: $black;
            font-size:14px;
        }
    }
    .card-list {
        display: flex;
        justify-content: space-between;
        margin-top: 40px;
    }
    .content:last-child {
        margin-top: 59px;
    }
</style>