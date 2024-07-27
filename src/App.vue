<template>
  <section class="w-100 section-one p-0 row position-absolute z-0">
    <div class="shadow shadow-one"></div>
    <div class="col-8">
      <img src="./assets/imgs/shape1.png" alt="" class="w-100">
    </div>
  </section>
  <section class="container position-relative z-1">
    <div class="row pt-4">
      <div class="col-6 d-flex justify-content-center">
        <navBar />
      </div>
      <div class="col-6 d-flex justify-content-end align-items-center">
        <div class="dropdown dropdown-profile">
          <button class="dropdown-profile-btn btn btn-secondary dropdown-toggle rounded-pill border-0 py-2"
            type="button" data-bs-toggle="dropdown" aria-expanded="false" dir="rtl">
            <img src="./assets/imgs/profilImg.png" class="mx-2" alt="">
            Dropdown button
          </button>
          <ul class="dropdown-menu w-100">
            <li><a class="dropdown-item text-light" href="#">account</a></li>
            <li><a class="dropdown-item text-light" href="#">Another action</a></li>
            <li><a class="dropdown-item text-light" href="#">log out</a></li>
          </ul>
        </div>
      </div>
    </div>
  </section>
  <section class="container mt-5 position-relative z-0">
    <div class="row pt-5">
      <viv class="col-6 text-center">
        <img class="w-50 position-relative z-0" src="./assets/imgs/coin.png" alt="">
        <img class="w-100" src="./assets/imgs/shape2.png" alt="">
      </viv>
      <viv class="col-6">
        <h1 class="h1 text-light">
          BUILD YOUR <span class="header-text-primary">FUTURE</span>
        </h1>
        <p class="text-light mt-4">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore
          magna aliqua
        </p>
        <div class="d-flex justify-content-end gap-4 mt-5">
          <button type="button" class="btn header-btn header-btn-primary rounded-pill">GET STARTED</button>
          <button type="button" class="btn header-btn btn-outline-light rounded-pill">DOWNLOD APP</button>
        </div>
      </viv>
    </div>
  </section>
  <section class="w-100 section-one p-0 row position-absolute z-0 d-flex justify-content-end">
    <div class="shadow shadow-tow"></div>
    <div class="col-4">
      <img src="./assets/imgs/shape3.png" alt="" class="w-100 h-50 shadow-tow--img">
    </div>
  </section>
  <section class="container mt-5 position-relative">
    <div>
      <inputTitle :classes="['text-center', 'py-4']" color="#fff" text="TOP CURRENCIES" />
      <p class="text-center text-light" style="font-size: 13px; margin-top: -20px">Lorem ipsum dolor sit amet,
        consectetur adipiscing elit</p>
    </div>
    <div class="table-box py-3 px-4 rounded-5">
      <CriptoTable :body="cryptodata" />
    </div>
  </section>
  <section class="container mt-5">
    <div class="pt-3">
      <inputTitle :classes="['text-center', 'py-4','mt-5']" color="#fff" text="LET’S SEE HOW IT WORKS" />
      <p class="text-center text-light" style="font-size: 16px; margin-top: -20px">Lorem ipsum dolor sit amet,
        consectetur adipiscing elit, sed do <br>eiusmod tempor incididunt ut labore et dolore magna aliqua</p>
    </div>
    <div class="d-flex justify-content-center w-100 mt-5">
      <div class="w-75">
        <img src="./assets/icon/lineVector1.png" class="w-100" style="margin-bottom: -110px;" alt="">
        <div class="d-flex justify-content-between">
          <div>
            <img src="./assets/icon/createAcont.png" alt="">
          </div>
          <div>
            <img src="./assets/icon/fingerPrint.png" alt="">
          </div>
          <div>
            <img src="./assets/icon/wallet.png" alt="">
          </div>
        </div>
      </div>
    </div>
    <div class="row justify-content-around  w-100 mt-5">
      <div class="col text-center text-light">
        <span class="ps-4 fw-bold fs-5"> CREATE AN ACCOUNT </span>
        <p style="font-size: 13px;" class="ps-4 mt-2"> Lorem ipsum dolor sit amet, consectetur adipiscing elit </p>
      </div>
      <div class="col text-center text-light ps-5">
        <span class="fw-bold fs-5"> VERIFY </span>
        <p style="font-size: 13px;" class="mt-2"> Lorem ipsum dolor sit amet, consectetur adipiscing elit </p>
      </div>
      <div class="col text-center text-light ps-4">
        <span class="ps-4 fw-bold fs-5"> CONNECT BANK ACCOUNT </span>
        <p style="font-size: 13px;" class="ps-4 mt-2"> Lorem ipsum dolor sit amet, consectetur adipiscing elit </p>
      </div>
    </div>
  </section>
  <section class="w-100 section-one p-0 row position-absolute z-0 d-flex justify-content-start">
    <div class="shadow shadow-three"></div>
    <div class="col-5">
      <img src="./assets/imgs/shape4.png" alt="" class="w-100 h-75 shadow-three--img">
    </div>
  </section>
  <section class="container mt-5 z-1">
    <div class="pt-5">
      <inputTitle :classes="['text-center', 'py-4','mt-5']" color="#fff" text="HOW TO INVEST?" />
      <p class="text-center text-light" style="font-size: 16px; margin-top: -20px">Lorem ipsum dolor sit amet,
        consectetur adipiscing elit, sed do <br>eiusmod tempor incididunt ut labore et dolore magna aliqua</p>
    </div>
    <div class="d-flex justify-content-center w-100 mt-5">
      <div class="w-75">
        <img src="./assets/icon/lineVector2.png" class="w-100" style="margin-bottom: -110px;" alt="">
      </div>
    </div>
    <div class="row justify-content-around  w-100 mt-5">
      <div class="col text-center text-light">
        <span class="ps-4 fw-bold fs-5"> CREATE AN ACCOUNT </span>
        <p style="font-size: 13px;" class="ps-4 mt-2"> Lorem ipsum dolor sit amet, consectetur adipiscing elit </p>
      </div>
      <div class="col text-center text-light ps-5">
        <span class="fw-bold fs-5"> VERIFY </span>
        <p style="font-size: 13px;" class="mt-2"> Lorem ipsum dolor sit amet, consectetur adipiscing elit </p>
      </div>
      <div class="col text-center text-light ps-4">
        <span class="ps-4 fw-bold fs-5"> CONNECT BANK ACCOUNT </span>
        <p style="font-size: 13px;" class="ps-4 mt-2"> Lorem ipsum dolor sit amet, consectetur adipiscing elit </p>
      </div>
    </div>
  </section>
  <section class="w-100 section-one p-0 row position-absolute z-0 d-flex justify-content-end">
    <div class="shadow shadow-four"></div>
  </section>
  <section class="container mt-5 py-5">
    <img src="./assets/imgs/appleImg.jpg" class="position-relative w-100 rounded-5 mt-5" alt="">
  </section>
  <section class="w-100 section-one p-0 row position-absolute z-0">
    <div class="shadow shadow-five"></div>
  </section>
  <section class="container my-5">
    <div class="pt-5">
      <inputTitle :classes="['text-center', 'py-4']" color="#fff" text="Frequently Asked Questions" :size="'2.5rem'" />
      <accordion :data="data" :fontSize="'27px'" />
    </div>
  </section>
  <section class="container mt-5 py-3">
    <footer class="nav-bar--footer d-flex justify-content-between ps-1">
      <div>
        <img src="./assets/icon/shape1.png" alt="">
      </div>
      <div>
        <ul class="d-flex gap-4">
          <li><a class="text-light" href="#">HOME</a></li>
          <li><a class="text-light" href="#">VALLETS</a></li>
          <li><a class="text-light" href="#">NFTS</a></li>
          <li><a class="text-light" href="#">BUY</a></li>
          <li><a class="text-light" href="#">FARMS</a></li>
        </ul>
      </div>
    </footer>
  </section>
</template>

<script setup>
import './assets/css/mainPage.scss'
import accordion from './components/inputs/Accordion.vue';
import inputTitle from './components/inputs/InputTitle.vue';
import navBar from './components/NavBar.vue';
import CriptoTable from './components/CriptoTable.vue';
import { ref, defineProps, onMounted } from 'vue';
const data = ref([
  { title: '1.Frequently Asked Questions', description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna liqua', iconSrc: '/src/assets/icon/close.png' },
  { title: '2.Frequently Asked Questions', description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna liqua', iconSrc: '/src/assets/icon/close.png' },
  { title: '3.Frequently Asked Questions', description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna liqua', iconSrc: '/src/assets/icon/close.png' },
  { title: '4.Frequently Asked Questions', description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna liqua', iconSrc: '/src/assets/icon/close.png' }
])
const cryptodata = ref([
  { nemeSrc: '', name: 'bitcoin', price: 33.59, change: 25, market: 653.14 },
  { nemeSrc: '', name: 'bitcoin', price: 33.59, change: -25, market: 653.14 },
  { nemeSrc: '', name: 'bitcoin', price: 33.59, change: 25, market: 653.14 },
  { nemeSrc: '', name: 'bitcoin', price: 33.59, change: 0, market: 653.14 },
  { nemeSrc: '', name: 'bitcoin', price: 33.59, change: 25, market: 653.14 },
  { nemeSrc: '', name: 'bitcoin', price: 33.59, change: 25, market: 653.14 },
  { nemeSrc: '', name: 'bitcoin', price: 33.59, change: -25, market: 653.14 },
  { nemeSrc: '', name: 'bitcoin', price: 33.59, change: 25, market: 653.14 }
])
</script>
<style scoped lang="scss"></style>
