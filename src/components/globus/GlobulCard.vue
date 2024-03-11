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
  height: 100%;
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
  background: #20ce701a;
  box-shadow: 0px 0px 28.425865173339844px 0px #14141480;
  border-radius: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
}
.globus-box h2 {
  font-size: 30px;
  font-weight: 400;
  line-height: 48px;
  letter-spacing: 0em;
  color: var(--green-800) !important;
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
  animation: anima3 5s infinite;
  animation-delay: 3s;
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
  animation: anima2 5s infinite;
  animation-delay: 1s;
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
  animation: anima1 5s infinite;
}
@keyframes anima3 {
  0% {
    border-color: #207748;
  }
  50% {
    border-color: #20ce701a;
  }
  100% {
    border-color: #207748;
  }
}
@keyframes anima2 {
  0% {
    border-color: #207748;
  }
  50% {
    border-color: #20ce701a;
  }
  100% {
    border-color: #207748;
  }
}
@keyframes anima1 {
  0% {
    border-color: #207748;
  }
  50% {
    border-color: #20ce701a;
  }
  100% {
    border-color: #207748;
  }
}

.globus-card h2 {
  color: #fff;
}

@media (max-width: 1400px) {
  .globus-card-left ul li:nth-child(2) {
    padding-left: 30px;
    padding-right: 30px;
  }
  .globus-box {
    height: 155px;
    width: 155px;
  }
  .globus-box h2 {
    font-size: 28px;
    line-height: 36px;
  }
}
@media (max-width: 1200px) {
  .globus-card-left ul li:nth-child(2) {
    padding-left: 30px;
    padding-right: 30px;
  }
  .globus-box {
    height: 150px;
    width: 150px;
  }
  .globus-box h2 {
    font-size: 26px;
    line-height: 30px;
  }
}

@media (max-width: 991px) {
  .globus-card {
    padding: 10px 10px 10px 40px;
  }
  .globus-card ul {
    gap: 15px;
  }

  .globus-card-left ul li:nth-child(2) {
    padding-left: 15px;
    padding-right: 15px;
  }
  .globus-card-right {
    margin-right: 20px;
  }
  .globus-box {
    height: 140px;
    width: 140px;
  }
  .globus-box h2 {
    font-size: 22px;
    line-height: 26px;
  }
}

@media (max-width: 780px) {
  .globus-card ul {
    gap: 15px;
  }
  .globus-card-left ul li:nth-child(2) {
    padding-left: 20px;
    padding-right: 20px;
  }
  .globus-box {
    height: 140px;
    width: 140px;
  }
  .globus-card-right {
    margin-right: 10px;
  }
  .globus-box h2 {
    font-size: 25px;
    line-height: 30px;
  }
}

@media (max-width: 576px) {
  .globus-card {
    padding: 8px 8px 8px 40px;
    gap: 15px;
  }
  .globus-card-left {
    height: 120px !important;
  }
  .globus-card ul {
    gap: 10px;
  }
  .globus-card-left ul li:nth-child(2) {
    padding-left: 10px;
    padding-right: 10px;
  }
  .globus-box {
    height: 120px;
    width: 120px;
  }
  .line-one {
    width: 130%;
    height: 50%;
    top: 50%;
    left: -15%;
  }

  .line-two {
    width: 130%;
    left: -15%;
  }

  .line-three {
    width: 130%;
    left: -15%;
  }
  .globus-card-right {
    margin-right: 10px;
  }
  .globus-box h2 {
    font-size: 20px;
    line-height: 25px;
  }
}
</style>
