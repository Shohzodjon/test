<script lang="ts" setup></script>
<template>
<div class="globus-card">
<div class="globus-card-left">
    <h4 class="sub-title">Waxpeer online & status</h4>
    <ul>
        <li>
            <h3 class="main-title">12698</h3>
            <span class="desc-par">extension</span>
        </li>
        <li>
            <h3 class="main-title">5898</h3>
            <span class="desc-par">desktop</span>
        </li>
        <li>
            <h3 class="main-title">25697</h3>
            <span class="desc-par">mobile</span>
        </li>
    </ul>
</div>
<div class="globus-card-right">

    <div class="globus-box">
        <h2>Stable</h2>
        <span class="line-one"></span>
        <span class="line-two"></span>
        <span class="line-three"></span>
    </div>

</div>
</div>

</template>
<style scoped>
.globus-card{
    border: 1px solid red;
    display: flex;
    padding:10px 10px 10px 42px;
    justify-content: space-between;
    align-items: center;
}
.globus-card ul{
    list-style: none;
    margin:0 !important;
    padding: 0;
}
.globus-box{
    height: 163.76px;
    width: 163.76px;
    background: #20CE701A;
    box-shadow: 0px 0px 28.425865173339844px 0px #14141480;
}
.globus-card h2{
    color: #fff;
}
</style>