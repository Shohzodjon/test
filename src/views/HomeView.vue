<script setup lang="ts">
import ChartCart from '@/components/chart-card/ChartCart.vue';
import CardComp from '@/components/CardComp.vue';
import UpIcon from '@/assets/icons/UpIcon.vue';
import BitCoin from '@/assets/icons/BitCoin.vue';
import DollarSign from '@/assets/icons/DollarSign.vue';
import DoubleArrow from '@/assets/icons/DoubleArrow.vue';
import CalendarIcon from '@/assets/icons/CalendarIcon.vue';
import Machine from '@/assets/icons/Machine.vue';
import Cloud from '@/assets/icons/Cloud.vue';
import Store from '@/assets/icons/Store.vue';
import Settings from '@/assets/icons/Settings.vue';
import Login from '@/assets/icons/Login.vue';
import PayIcon from '@/assets/icons/PayIcon.vue';
import Logo from '@/assets/icons/Logo.vue';
import { RouterLink } from 'vue-router';
</script>

<template>
  <section>
    <div class="container">
      <div class="box-wrapper">
        <RouterLink to="/">
          <Logo />
        </RouterLink>
        <div class="card-grid">
          <div class="grid-item">
            <ChartCart />
          </div>
          <div class="grid-item">
            <CardComp sub-title="Current date" desc-par="Current date and time" btn-class="main-class">
              <template #button-slot>
                <UpIcon />
              </template>

              <template #card-bottom>
                <div class="date-bottom">
                  <h3 class="main-title">08.06.2022</h3>
                  <span>19:55:20</span>
                </div>
              </template>
            </CardComp>
          </div>
          <!--  -->
          <div class="grid-item">
            <CardComp sub-title="Withdrawal status" desc-par="Connected cryptocurrencies" btn-class="main-class">

              <template #button-slot>
                <BitCoin />
              </template>

              <template #card-bottom>
                <ul class="kripto-list">
                  <li>
                    <img src="@/assets/images/ton.png" alt="tether">
                  </li>
                  <li>
                    <img src="@/assets/images/ton2.png" alt="ton2">
                  </li>
                  <li>
                    <img src="@/assets/images/ton3.png" alt="ton3">
                  </li>
                </ul>
              </template>
            </CardComp>
          </div>
          <div class="grid-item">
            <CardComp sub-title="Buy items" desc-par="Time from the last purchase" btn-class="main-class">

              <template #button-slot>
                <DollarSign />
              </template>

              <template #card-bottom>
                <div class="buy-bottom">
                  <h3 class="main-title">25 sec</h3>
                </div>
              </template>
            </CardComp>
          </div>

          <div class="grid-item">
            <CardComp sub-title="Waxpeer pay bots" desc-par="The number of avaliable bots on Wxpeer pay"
              btn-class="main-class">

              <template #button-slot>
                <DoubleArrow />
              </template>

              <template #card-bottom>
                <div class="pay-bots-bottom">
                  <h3 class="main-title">259 bots</h3>
                </div>
              </template>
            </CardComp>
          </div>

          <div class="grid-item">

            <CardComp sub-title="Waxpeer pay" desc-par="The last successful trade" btn-class="main-class">

              <template #button-slot>
                <PayIcon />
              </template>

              <template #card-bottom>
                <div class="buy-bottom">
                  <h3 class="main-title">10 sec</h3>
                </div>
              </template>
            </CardComp>
          </div>

          <div class="grid-item">
            <CardComp sub-title="Availability of a site" desc-par="The availability of the home page of the site"
              btn-class="aviable-btn">

              <template #button-slot>
                <CalendarIcon />
              </template>

              <template #card-bottom>
                <div class="">
                  <h3 class="aviable-title">available</h3>
                </div>
              </template>
            </CardComp>
          </div>

          <div class="grid-item">
            <CardComp sub-title="Server status" desc-par="The status of the website servers" btn-class="server-btn">

              <template #button-slot>
                <Cloud />
              </template>

              <template #card-bottom>
                <div>
                  <h3 class="server-title">unstable</h3>
                </div>
              </template>
            </CardComp>
          </div>

          <div class="grid-item">
            <CardComp sub-title="Steam Web API" desc-par="Last check June 3, 2022 02:50:16" btn-class="stream-btn">

              <template #button-slot>
                <Machine />
              </template>

              <template #card-bottom>
                <div>
                  <h3 class="stream-title">stable</h3>
                </div>
              </template>
            </CardComp>
          </div>

          <div class="grid-item">
            <CardComp sub-title="API response" desc-par="Last request 10 seconds ago" btn-class="main-class">

              <template #button-slot>
                <Settings />
              </template>

              <template #card-bottom>
                <div class="buy-bottom">
                  <h3 class="main-title">2.856 ms</h3>
                </div>
              </template>
            </CardComp>
          </div>

          <div class="grid-item">
            <CardComp sub-title="Last trade" desc-par="The last trade was created 5s ago" btn-class="store-btn">

              <template #button-slot>
                <Store />
              </template>

              <template #card-bottom>
                <div>
                  <h3 class="trade-title">canceled</h3>
                </div>
              </template>
            </CardComp>
          </div>

          <div class="grid-item">
            <CardComp sub-title="Login" desc-par="Shows either your login is working or not" btn-class="login-btn">

              <template #button-slot>
                <Login />
              </template>

              <template #card-bottom>
                <div>
                  <h3 class="login-title">active</h3>
                </div>
              </template>
            </CardComp>
          </div>

        </div>
      </div>

    </div>
  </section>
</template>

<style scoped>
section {
  background: var(--black-900);
  height: 100%;
}

.box-wrapper {
  padding: 6px;
}

.box-wrapper a {
  margin-bottom: 25px;
  display: block;
}

.card-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 15px;
}

.date-bottom {
  display: flex;
  align-items: center;
  justify-content: space-between;
}




/* extra style */
.date-bottom span {
  font-size: 20px;
  font-weight: 400;
  line-height: 32px;
  letter-spacing: 0em;
  color: #BABAC280;
}

.kripto-list {
  display: flex;
  align-items: center;
  justify-content: flex-end;
  gap: 10px;
}

.kripto-list li {
  width: 46.87px;
  height: 46.87px;
  list-style: none;
  cursor: pointer;
}

.kripto-list li img {
  width: 100%;
  height: 100%;
}

.buy-bottom {
  display: flex;
  justify-content: flex-end;
}

.pay-bots-bottom {
  display: flex;
  justify-content: flex-end;
}

.aviable-title,
.server-title,
.stream-title,
.trade-title,
.login-title {
  text-align: right;
  font-size: 30px;
  font-weight: 400;
  line-height: 48px;
  letter-spacing: 0em;
  color: var(--green-800);
}

.server-title {
  color: #EC7A2A !important;
}

.trade-title {
  color: #EF5858;
}
</style>

<style>
.aviable-btn,
.stream-btn,
.login-btn {
  background: #20CE7012 !important;
}

.server-btn {
  background: #EC7A2A12 !important;
}

.store-btn {
  background: #EF585812 !important;
}
</style>
