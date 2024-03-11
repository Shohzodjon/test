<script lang="ts" setup>
import UpIcon from '@/assets/icons/UpIcon.vue';
</script>

<template>
    <div class="chart-card">
        <div class="card-header">
            <button>
                <UpIcon />
            </button>
            <div class="header-right">
                <h4 class="sub-title">Uptime</h4>
                <p class="desc-par">Uptime over the past 24 hours</p>
            </div>

        </div>

        <div class="cart-status">
            <h3 class="main-title">97.83%</h3>
            <img src="@/assets/images/chart.svg" alt="chart">
        </div>
    </div>
</template>

<style scoped>
.chart-card {
    background: var(--black-700);
    border-radius: 8px;
    padding: 12px;
    box-sizing: border-box;
    height: 100%;
}

.card-header {
    display: flex;
    align-items: flex-start;
    gap: 10px;
    margin-bottom: 20px;
}

.card-header button {
    border: none;
    height: 32px;
    width: 32px;
    background: #262626;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 100%;
    cursor: pointer;
}

.header-right {
    display: flex;
    flex-direction: column;
    gap: 10px;
    padding-top: 4px;
}

.cart-status {
    display: flex;
    align-items: center;
    margin-left: 42px;
    width: auto;
    justify-content: space-between;
}
.cart-status img{
    height: 55.6px;
}
</style>