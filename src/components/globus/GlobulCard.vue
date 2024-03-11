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
.globus-card {
    display: flex;
    padding: 10px 10px 10px 42px;
    justify-content: space-between;
    align-items: stretch;
    max-height: 200px;
}

.globus-card-left {
    display: flex;
    flex-direction: column;
    height: 140px !important;
    justify-content: space-between;
}

.globus-card ul {
    list-style: none;
    margin: 0 !important;
    padding: 0;
    display: flex;
    align-items: center;
    gap: 20px;
}

.globus-card-left ul li:nth-child(2) {
    padding-left: 40px;
    padding-right: 40px;
    border-left: 1.35px solid #333333;
    border-right: 1.35px solid #333333;

}

.globus-card-right {
    margin-right: 30px;
}

.globus-box {
    height: 163.76px;
    width: 163.76px;
    background: #20CE701A;
    box-shadow: 0px 0px 28.425865173339844px 0px #14141480;
    border-radius: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    position: relative;
}

.line-one {
    position: absolute;
    width: 135%;
    height: 50%;
    top: 50%;
    left: -17.5%;
    border: 1px solid #207748;
    border-radius: 46% !important;
    overflow: hidden;
    transform: translateY(-50%) rotate(-38deg);
    overflow: hidden;
}

.line-two {
    position: absolute;
    width: 135%;
    height: 54%;
    top: 50%;
    left: -17.5%;
    border: 1px solid #207748;
    border-radius: 48%;
    transform: translateY(-50%) rotate(66deg);
    transform-origin: center;
}

.line-three {
    position: absolute;
    width: 135%;
    height: 50%;
    top: 50%;
    left: -17.5%;
    border: 1px solid #207748;
    border-radius: 46%;
    transform: translateY(-50%) rotate(15deg);
    transform-origin: center;
    animation: mymove 5s infinite;
}

@keyframes mymove {
    0% {
        border-color: #207748;
    }
    50%{
        border-color: #20CE701A;
    }
    100% {
        border-color:#207748 ;
    }
}


.globus-card h2 {
    color: #fff;
}
</style>