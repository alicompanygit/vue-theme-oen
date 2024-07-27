<template>
  <section class="border-bottom">
    <nav class="navbar navbar-expand-lg bg-body-tertiary d-flex justify-content-between">
      <div class="px-3 py-2">
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavAltMarkup"
          aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
          <div class="navbar-nav">
            <a class="nav-link d-none d-lg-block" href="#"><img src="./assets/imgs/a1.png" alt=""></a>
            <a class="nav-link fs-6 fw-bold" href="#">صفحه اصلی</a>
            <a class="nav-link fs-6 fw-bold" href="#">درباره ما</a>
            <a class="nav-link fs-6 fw-bold" href="#">خدمات</a>
            <a class="nav-link fs-6 fw-bold" href="#">تماس باما</a>
            <a class="nav-link fs-6 fw-bold" href="#">پلن ها</a>
          </div>
        </div>
      </div>
      <div class="px-3 py-2">
        <!-- <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent"
          aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button> -->
        <div class=" navbar-collapse">
          <ul class="navbar-nav me-auto mb-2 mb-lg-0 align-items-center mt-2">
            <li class="nav-item dropdown d-flex">
              <a class="nav-link dropdown-toggle fs-6" href="#" role="button" data-bs-toggle="dropdown"
                aria-expanded="false">
                <img src="./assets/imgs/a2.png" alt="" class="ronded  rounded-circle ms-2"
                  style="width: 30px; height: 30px">
                <span>
                  ali nodryan
                </span>
              </a>
              <ul class="dropdown-menu">
                <li><a class="dropdown-item" href="#">پروفایل</a></li>
                <li><a class="dropdown-item" href="#">خروج</a></li>
              </ul>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </section>
  <section class="container mt-5">
    <div class="row">
      <div class="col">
        <div class="d-flex justify-content-between">
          <img src="./assets/icon/a6.png" alt="" style="width: 70px; height: 70px; margin-top: 100px"
            class="z-1 shape1">
          <img src="./assets/icon/a7.png" alt="" style="width: 70px; height: 70px;" class="ms-4 z-1 shape2">
        </div>
        <div class="d-flex justify-content-end">
          <img src="./assets/icon/a8.png" alt="" style="width: 50px; height: 70px;" class="z-1 shape3">
        </div>
        <img src="./assets/imgs/a3.jpg" alt="" style="margin-top: -240px;" class="z-0">
      </div>
      <div class="col mt-5">
        <h1 class="mt-5">
          زمانتو مدیریت نکن....! <br>
          زمانتو بخر...!
        </h1>
        <p class="mt-5">
          لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است
        </p>
        <div class="pt-5" @mouseleave="systemActiv = false">
          <div v-if="systemActiv" class="border position-absolute rounded-4"
            style="margin-top: -160px; background-color: #fff;">
            <div class="row p-5 gap-4">
              <div class="col text-center p-2 px-4 rounded-4 mac">
                <img src="./assets/icon/a22.png" alt="" style="width: 50px;" class="systemsImg mb-2"
                  @mouseenter="setQRcod($event, true, '', '.mac')"
                  @mouseleave="setQRcod($event, false, '/src/components/projectOne/assets/icon/a22.png', '.mac')"><br>
                <span style="font-size: 14px;">MAC</span>
              </div>
              <div class="col text-center p-2 rounded-4 windows">
                <img src="./assets/icon/a24.png" alt="" style="width: 50px;" class="systemsImg mb-2"
                  @mouseenter="setQRcod($event, true, '', '.windows')"
                  @mouseleave="setQRcod($event, false, '/src/components/projectOne/assets/icon/a24.png', '.windows')"><br>
                <span style="font-size: 14px;">WINDOWS</span>
              </div>
              <div class="col text-center p-2 px-3 rounded-4 android">
                <img src="./assets/icon/a23.png" alt="" style="width: 43px;" class="systemsImg mb-2"
                  @mouseenter="setQRcod($event, true, '', '.android')"
                  @mouseleave="setQRcod($event, false, '/src/components/projectOne/assets/icon/a23.png', '.android')"><br>
                <span style="font-size: 14px;">ANDROID</span>
              </div>
              <div class="col text-center p-2 px-4 rounded-4 ios">
                <img src="./assets/icon/a25.png" alt="" style="width: 41px;" class=" mb-2"
                  @mouseenter="setQRcod($event, true, '', '.ios')"
                  @mouseleave="setQRcod($event, false, '/src/components/projectOne/assets/icon/a25.png', '.ios')"><br>
                <span style="font-size: 14px;">IOS</span>
              </div>
            </div>
          </div>
          <div class="d-flex justify-content-center gap-2 mt-5">
            <button type="button" class="btn1 btn1-f btn btn-outline-primary rounded-pill w-50 gap-1"
              @mouseenter="systemActiv = true">دانلود نرم افزار
              <img src="./assets/icon/a4.svg" alt="" style="width: 18px;"></button>
            <button @mouseenter="systemActiv = false" type="button" class="btn1 btn1-s btn rounded-pill w-50 gap-2">ثبت
              نام کن <img src="./assets/icon/a5.svg" alt="" style="width: 7px;"></button>
          </div>
        </div>
      </div>
    </div>
    <div class="box row">
      <div class="col p-5 box-data rounded-end-5">
        <div class="text-center fs-5 fw-bold">
          +5میلیون کاربر
        </div>
        <div class="text-center fs-6 opacity-75">
          کابر فعال
        </div>
      </div>
      <div class="col p-5 box-data">
        <div class="text-center fs-5 fw-bold">
          500هزار
        </div>
        <div class="text-center fs-6 opacity-75">
          تیم فعال
        </div>
      </div>
      <div class="col p-5 box-data">
        <div class="text-center fs-5 fw-bold">
          +40 هزار
        </div>
        <div class="text-center fs-6 opacity-75">
          شرکت معتبر
        </div>
      </div>
      <div class="col p-5 box-data rounded-start-5">
        <div class="text-center fs-5 fw-bold">
          +۵ میلیون
        </div>
        <div class="text-center fs-6 opacity-75">
          کاربر فعال
        </div>
      </div>
    </div>
  </section>
  <section class="container mt-5 pt-5">
    <div class="row pt-5">
      <div class="col earth">
        <div class="w-100 d-flex justify-content-center">
          <img src="./assets/imgs/a9.jpg" alt="" style="width: 400px;" class="earth-img">
        </div>
        <div class="d-flex justify-content-center">
          <div>
            <div class="earth-items-1 d-flex justify-content-center">
              <div class="text-center">
                <div style="margin-bottom: -63px;">
                  <img class="earth-pa" src="./assets/imgs/a14.png" style="width: 90px;" alt="">
                </div>
                <img src="./assets/imgs/a10.png" style="width: 30px; margin-bottom: -7px" alt="">
                <div class="text-center d-flex align-items-center justify-content-center">
                  <span style="font-size: 13px;" class="fw-bold">parham</span>
                  <span>
                    <img src="./assets/icon/a15.svg" style="width: 15px;" alt="">
                  </span>
                </div>
              </div>
            </div>
            <div class="earth-items-2 d-flex justify-content-center">
              <div class="text-center">
                <div style="margin-bottom: -63px;">
                  <img class="earth-pa" src="./assets/imgs/a14.png" style="width: 90px;" alt="">
                </div>
                <img src="./assets/imgs/a10.png" style="width: 30px; margin-bottom: -7px" alt="">
                <div class="text-center d-flex align-items-center justify-content-center">
                  <span style="font-size: 13px;" class="fw-bold">parham</span>
                  <span>
                    <img src="./assets/icon/a15.svg" style="width: 15px;" alt="">
                  </span>
                </div>
              </div>
            </div>
            <div class="earth-items-3 d-flex justify-content-center">
              <div class="text-center">
                <div style="margin-bottom: -63px;">
                  <img class="earth-pa" src="./assets/imgs/a14.png" style="width: 90px;" alt="">
                </div>
                <img src="./assets/imgs/a10.png" style="width: 30px; margin-bottom: -7px" alt="">
                <div class="text-center d-flex align-items-center justify-content-center">
                  <span style="font-size: 13px;" class="fw-bold">parham</span>
                  <span>
                    <img src="./assets/icon/a15.svg" style="width: 15px;" alt="">
                  </span>
                </div>
              </div>
            </div>
            <div class="earth-items-4 d-flex justify-content-center">
              <div class="text-center">
                <div style="margin-bottom: -63px;">
                  <img class="earth-pa" src="./assets/imgs/a14.png" style="width: 90px;" alt="">
                </div>
                <img src="./assets/imgs/a10.png" style="width: 30px; margin-bottom: -7px" alt="">
                <div class="text-center d-flex align-items-center justify-content-center">
                  <span style="font-size: 13px;" class="fw-bold">parham</span>
                  <span>
                    <img src="./assets/icon/a15.svg" style="width: 15px;" alt="">
                  </span>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="col d-flex align-items-center">
        <div>
          <h2 class="fw-bold h3">از هر جای دنیا تیمتو مدیریت کن</h2>
          <p class="mt-5 earth-text">
            لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است چاپگرها و متون
            بلکه روزنامه و مجله در ستون و سطرآنچنان که لازم است و برای شرایط فعلی تکنولوژی مورد نیاز و کاربردهای متنوع
            با
            هدف بهبود ابزارهای کاربردی می باشد
          </p>
          <div class="w-100 d-flex justify-content-end mt-5">
            <button type="button" class="btn1 btn1-f btn btn-outline-primary rounded-pill w-50">تشکیل تیم</button>
          </div>
        </div>
      </div>
    </div>
  </section>
  <section class="container mt-5 sec4">
    <div class="w-100 d-flex justify-content-center pt-5">
      <h2 class="fw-bold mt-5">چرا ما باید انتخاب شما باشیم؟</h2>
    </div>
    <div class="row">
      <div class="col-12 col-lg">
        <div class="z-0 position-absolute">
          <span style="font-size: 230px; color: rgba(232, 232, 255, 1)">۱</span>
        </div>
        <div class="pe-3 z-1 position-relative" style="margin-top: 70px;">
          <h4 class="fs-6 fw-bold se4-title">لورم ایپسوم متن ساختگی نامفهوم</h4>
          <p class="mt-3 text-wrap">
            لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است چاپگرها و متون
            بلکه روزنامه و مجله در ستون و سطرآنچنان که لازم است
          </p>
        </div>
      </div>
      <div class="col-12 col-lg">
        <div class="z-0 position-absolute">
          <span style="font-size: 230px; color: rgba(232, 232, 255, 1)">۲</span>
        </div>
        <div class="pe-3 z-1 position-relative" style="margin-top: 70px;">
          <h4 class="fs-6 fw-bold se4-title">لورم ایپسوم متن ساختگی نامفهوم</h4>
          <p class="mt-3 text-wrap">
            لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است چاپگرها و متون
            بلکه روزنامه و مجله در ستون و سطرآنچنان که لازم است
          </p>
        </div>
      </div>
      <div class="col-12 col-lg">
        <div class="z-0 position-absolute">
          <span style="font-size: 230px; color: rgba(232, 232, 255, 1)">۳</span>
        </div>
        <div class="pe-3 z-1 position-relative" style="margin-top: 70px;">
          <h4 class="fs-6 fw-bold se4-title">لورم ایپسوم متن ساختگی نامفهوم</h4>
          <p class="mt-3 text-wrap">
            لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است چاپگرها و متون
            بلکه روزنامه و مجله در ستون و سطرآنچنان که لازم است
          </p>
        </div>
      </div>
    </div>
  </section>
  <section class="container mt-6">
    <inputTitle :text="'کار با بهترین هارا با ما تجربه کنید'" :classes="['text-center', 'pt-5', 'mt-5']" class="">
    </inputTitle>
  </section>
  <section class="mt-5 sec5 d-none d-xl-block">
    <div class="w-100 sec5-background">
      <h2 style="color: #fff; font-size: 300px; margin-top: 130px; margin-bottom: -450px"
        class="opacity-50 text-center z-0 position-relative fw-bold">MAG</h2>
      <section class="container">
        <div class="z-1 position-relative">
          <div class="d-flex justify-content-center gap-5">
            <div class="my-theme my-theme__item1 d-flex justify-content-center align-items-end">
              <div>
                <div class="my-theme--text1" style="visibility: hidden;">
                  <span class="text-light fs-5 pe-2 fw-bold">گلنار پاکدوست</span>
                  <p class="ps-5 fw-bold text-light" style="font-size: 8px; padding-right: 0.7rem">
                    لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است چاپگرها
                    و متون بلکه روزنامه و مجله در ستون و سطرآنچنان که لازم است
                  </p>
                </div>
                <div style="margin-top: -38px;" class="d-flex align-items-end justify-content-center">
                  <div class="d-flex justify-content-cente pb-2" @click="showMor($event, '1'), showLess()">
                    <img src="./assets/imgs/a27.svg" style="width: 40px;" alt="" class="my-theme--shape1">
                  </div>
                </div>
              </div>
            </div>
            <div class="my-theme my-theme__item2 d-flex justify-content-center align-items-end">
              <div>
                <div class="my-theme--text2" style="visibility: hidden;">
                  <span class="text-light fs-5 pe-2 fw-bold">پارسا رادفرد</span>
                  <p class="ps-5 fw-bold text-light" style="font-size: 8px; padding-right: 0.7rem">
                    لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است چاپگرها
                    و متون بلکه روزنامه و مجله در ستون و سطرآنچنان که لازم است
                  </p>
                </div>
                <div style="margin-top: -38px;" class="d-flex align-items-end justify-content-center">
                  <div class="d-flex justify-content-cente pb-2" @click="showMor($event, '2'), showLess()">
                    <img src="./assets/imgs/a27.svg" style="width: 40px;" alt="" class="my-theme--shape2">
                  </div>
                </div>
              </div>
            </div>
            <div class="my-theme my-theme__item3 d-flex justify-content-center align-items-end">
              <div>
                <div class="my-theme--text3" style="visibility: hidden;">
                  <span class="text-light fs-5 pe-2 fw-bold">ایناز عزیزی</span>
                  <p class="ps-5 fw-bold text-light" style="font-size: 8px; padding-right: 0.7rem">
                    لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است چاپگرها
                    و متون بلکه روزنامه و مجله در ستون و سطرآنچنان که لازم است
                  </p>
                </div>
                <div style="margin-top: -38px;" class="d-flex align-items-end justify-content-center">
                  <div class="d-flex justify-content-cente pb-2" @click="showMor($event, '3'), showLess()">
                    <img src="./assets/imgs/a27.svg" style="width: 40px;" alt="" class="my-theme--shape3">
                  </div>
                </div>
              </div>
            </div>
            <div class="my-theme my-theme__item4 d-flex justify-content-center align-items-end">
              <div>
                <div class="my-theme--text4" style="visibility: hidden;">
                  <span class="text-light fs-5 pe-2 fw-bold">پارسا رادفرد</span>
                  <p class="ps-5 fw-bold text-light" style="font-size: 8px; padding-right: 0.7rem">
                    لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است چاپگرها
                    و متون بلکه روزنامه و مجله در ستون و سطرآنچنان که لازم است
                  </p>
                </div>
                <div style="margin-top: -38px;" class="d-flex align-items-end justify-content-center">
                  <div class="d-flex justify-content-cente pb-2" @click="showMor($event, '4'), showLess()">
                    <img src="./assets/imgs/a27.svg" style="width: 40px;" alt="" class="my-theme--shape4">
                  </div>
                </div>
              </div>
            </div>
            <div class="my-theme my-theme__item5 d-flex justify-content-center align-items-end">
              <div>
                <div class="my-theme--text5" style="visibility: hidden;">
                  <span class="text-light fs-5 pe-2 fw-bold">ایناز عزیزی</span>
                  <p class="ps-5 fw-bold text-light" style="font-size: 8px; padding-right: 0.7rem">
                    لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است چاپگرها
                    و متون بلکه روزنامه و مجله در ستون و سطرآنچنان که لازم است
                  </p>
                </div>
                <div style="margin-top: -38px;" class="d-flex align-items-end justify-content-center">
                  <div class="d-flex justify-content-cente pb-2" @click="showMor($event, '5'), showLess()">
                    <img src="./assets/imgs/a27.svg" style="width: 40px;" alt="" class="my-theme--shape5">
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
    </div>
  </section>
  <section class="container mt-6">
    <inputTitle :text="'بیشتر بخوانید و بیشتر بدانید'" :classes="['text-center']"></inputTitle>
  </section>
  <section class="mt-5 sec5">
    <div class="w-100 sec5-background">
      <h2 style="color: #fff; font-size: 300px; margin-top: 130px; margin-bottom: -450px"
        class="opacity-50 text-center z-0 position-relative fw-bold">MAG</h2>
      <section class="container">
        <div class="z-1 position-relative">
          <div class="row gap-5">
            <div class="col-12 col-lg p-0 pb-2 rounded-4" style="background-color: #fff;">
              <div class="d-flex justify-content-center">
                <img src="./assets/imgs/a16.jpg" alt="" class="w-100 sec5-img">
              </div>
              <div class="px-3">
                <h5 class="fw-bold text-center mt-4" style="font-size: 17px;">چرا ما باید انتخاب شما باشیم؟</h5>
                <p class="opacity-75 mt-2 text-center" style="font-size: 14px;">
                  لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است
                </p>
              </div>
            </div>
            <div class="col-12 col-lg p-0 pb-2 rounded-4" style="background-color: #fff;">
              <div class="d-flex justify-content-center">
                <img src="./assets/imgs/a17.jpg" alt="" class="w-100 sec5-img">
              </div>
              <div class="px-3">
                <h5 class="fw-bold text-center mt-4" style="font-size: 17px;">چرا ما باید انتخاب شما باشیم؟</h5>
                <p class="opacity-75 mt-2 text-center" style="font-size: 14px;">
                  لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است
                </p>
              </div>
            </div>
            <div class="col-12 col-lg p-0 pb-2 rounded-4" style="background-color: #fff;">
              <div class="d-flex justify-content-center">
                <img src="./assets/imgs/a18.jpg" alt="" class="w-100 sec5-img">
              </div>
              <div class="px-3">
                <h5 class="fw-bold text-center mt-4" style="font-size: 17px;">چرا ما باید انتخاب شما باشیم؟</h5>
                <p class="opacity-75 mt-2 text-center" style="font-size: 14px;">
                  لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است
                </p>
              </div>
            </div>
          </div>
          <div class="row gap-5 mt-5">
            <div class="col-12 col-lg p-0 pb-2 rounded-4" style="background-color: #fff;">
              <div class="d-flex justify-content-center">
                <img src="./assets/imgs/a18.jpg" alt="" class="w-100 sec5-img">
              </div>
              <div class="px-3">
                <h5 class="fw-bold text-center mt-4" style="font-size: 17px;">چرا ما باید انتخاب شما باشیم؟</h5>
                <p class="opacity-75 mt-2 text-center" style="font-size: 14px;">
                  لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است
                </p>
              </div>
            </div>
            <div class="col-12 col-lg p-0 pb-2 rounded-4" style="background-color: #fff;">
              <div class="d-flex justify-content-center">
                <img src="./assets/imgs/a16.jpg" alt="" class="w-100 sec5-img">
              </div>
              <div class="px-3">
                <h5 class="fw-bold text-center mt-4" style="font-size: 17px;">چرا ما باید انتخاب شما باشیم؟</h5>
                <p class="opacity-75 mt-2 text-center" style="font-size: 14px;">
                  لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است
                </p>
              </div>
            </div>
            <div class="col-12 col-lg p-0 pb-2 rounded-4" style="background-color: #fff;">
              <div class="d-flex justify-content-center">
                <img src="./assets/imgs/a17.jpg" alt="" class="w-100 sec5-img">
              </div>
              <div class="px-3">
                <h5 class="fw-bold text-center mt-4" style="font-size: 17px;">چرا ما باید انتخاب شما باشیم؟</h5>
                <p class="opacity-75 mt-2 text-center" style="font-size: 14px;">
                  لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است
                </p>
              </div>
            </div>
          </div>
        </div>
      </section>
    </div>
  </section>
  <section class="container mt-6">
    <inputTitle :text="'این نظرات شماست که مارا به سوی موفقیت سوق میدهد'" :classes="['text-center']"></inputTitle>
  </section>
  <section class="mt-5 sec5">
    <div class="w-100 sec5-background">
      <h2 style="color: #fff; font-size: 300px; margin-top: 130px; margin-bottom: -450px"
        class="opacity-50 text-center z-0 position-relative fw-bold">
        MAG
      </h2>
      <section class="container">
        <div class="z-1 position-relative">
          <div class="row gap-5">
            <div class="col-12 col-lg p-4 rounded-4" style="background-color: #fff; ">
              <div class="d-flex">
                <div>
                  <img src="./assets/imgs/a19.png" style="width: 55px;" alt="">
                </div>
                <div class="me-2">
                  <h6 class="fw-bold">ali nodryan</h6>
                  <img src="./assets/icon/a20.png" style="width: 60px; margin-top: -10px" alt="">
                </div>
              </div>
              <div>
                <p class="opacity-75 mt-2 text-center" style="font-size: 14px;">
                  لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است چاپگرها و
                  متون بلکه روزنامه و مجله در ستون و سطرآنچنان که لازم است و برای شرایط فعلی تکنولوژی مورد نیاز
                </p>
              </div>
            </div>
            <div class="col-12 col-lg p-4 rounded-4" style="background-color: #fff; ">
              <div class="d-flex">
                <div>
                  <img src="./assets/imgs/a19.png" style="width: 55px;" alt="">
                </div>
                <div class="me-2">
                  <h6 class="fw-bold">ali nodryan</h6>
                  <img src="./assets/icon/a20.png" style="width: 60px; margin-top: -10px" alt="">
                </div>
              </div>
              <div>
                <p class="opacity-75 mt-2 text-center" style="font-size: 14px;">
                  لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است چاپگرها و
                  متون بلکه روزنامه و مجله در ستون و سطرآنچنان که لازم است و برای شرایط فعلی تکنولوژی مورد نیاز
                </p>
              </div>
            </div>
            <div class="col-12 col-lg-3 p-4 rounded-4 d-flex justify-content-center align-items-center"
              style="background-color: #fff;">
              <div>
                <div class="d-flex justify-content-end ">
                  <img src="./assets/icon/a21.png" style="width: 40px;" alt="">
                </div>
                <div class="mt-2">
                  <h6 class="fw-bold" style="font-size: 30px;">امتیاز شما به ما</h6>
                </div>
                <div class="d-flex mt-2">
                  <h5>۴/۸</h5>
                  <img src="./assets/icon/a20.png" class="me-2" style="width: 120px; height: 20px" alt="">
                </div>
              </div>

            </div>
          </div>
          <div class="row gap-5 mt-5">
            <div class="col-12 col-lg p-4 rounded-4" style="background-color: #fff; ">
              <div class="d-flex">
                <div>
                  <img src="./assets/imgs/a19.png" style="width: 55px;" alt="">
                </div>
                <div class="me-2">
                  <h6 class="fw-bold">ali nodryan</h6>
                  <img src="./assets/icon/a20.png" style="width: 60px; margin-top: -10px" alt="">
                </div>
              </div>
              <div>
                <p class="opacity-75 mt-2 text-center" style="font-size: 14px;">
                  لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است چاپگرها و
                  متون بلکه روزنامه و مجله در ستون و سطرآنچنان که لازم است و برای شرایط فعلی تکنولوژی مورد نیاز
                </p>
              </div>
            </div>
            <div class="col-12 col-lg p-4 rounded-4" style="background-color: #fff; ">
              <div class="d-flex">
                <div>
                  <img src="./assets/imgs/a19.png" style="width: 55px;" alt="">
                </div>
                <div class="me-2">
                  <h6 class="fw-bold">ali nodryan</h6>
                  <img src="./assets/icon/a20.png" style="width: 60px; margin-top: -10px" alt="">
                </div>
              </div>
              <div>
                <p class="opacity-75 mt-2 text-center" style="font-size: 14px;">
                  لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است چاپگرها و
                  متون بلکه روزنامه و مجله در ستون و سطرآنچنان که لازم است و برای شرایط فعلی تکنولوژی مورد نیاز
                </p>
              </div>
            </div>
            <div class="col-12 col-lg p-4 rounded-4" style="background-color: #fff; ">
              <div class="d-flex">
                <div>
                  <img src="./assets/imgs/a19.png" style="width: 55px;" alt="">
                </div>
                <div class="me-2">
                  <h6 class="fw-bold">ali nodryan</h6>
                  <img src="./assets/icon/a20.png" style="width: 60px; margin-top: -10px" alt="">
                </div>
              </div>
              <div>
                <p class="opacity-75 mt-2 text-center" style="font-size: 14px;">
                  لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است چاپگرها و
                  متون بلکه روزنامه و مجله در ستون و سطرآنچنان که لازم است و برای شرایط فعلی تکنولوژی مورد نیاز
                </p>
              </div>
            </div>
          </div>
        </div>
      </section>
    </div>
  </section>
</template>

<script setup>
import inputTitle from '../inputs/InputTitle.vue';
import { computed, defineComponent, ref } from 'vue'
const systemActiv = ref(false)
function setQRcod(event, bool, img, clas) {
  if (bool == true) {
    document.querySelectorAll(clas).forEach((el) => [
      el.style.background = 'linear-gradient(#fff, #fff) padding-box,linear-gradient(269.79deg, #12A9E9 0.17%, #7371ED 66.43%) border-box',
      el.style.border = '2px solid transparent',
      el.style.borderRadius = '50px',
      el.style.padding = '10px 20px'
    ])
    event.target.setAttribute('src', '/src/components/projectOne/assets/icon/a26.png')
  } else {
    document.querySelectorAll(clas).forEach((el) => [
      el.style.removeProperty('background'),
      el.style.removeProperty('padding'),
      el.style.removeProperty('border-radius')
    ])
    event.target.setAttribute('src', img)
  }

}
const countWidth = ref(100)
const countWidthClose = ref(220)
const activ = ref('item')
const rotateOpen = ref(0)
const rotateClose = ref(0)
function showMor(event, item) {
  const interval = setInterval(() => {
    document.querySelectorAll(".my-theme__item" + item).forEach((el) => {
      countWidth.value++
      el.style.width = countWidth.value + 'px'
      if (countWidth.value > 222) {
        activ.value = item
        clearInterval(interval)
        countWidth.value = 100;
      }
    })
    document.querySelectorAll(".my-theme--shape" + item).forEach((shape) => {
      shape.style.transition = '0.70s'
      shape.style.transform = 'translateX(-80px) rotate(-225deg)'
    })
    document.querySelectorAll(".my-theme--text" + item).forEach((text) => {
      text.style.visibility = 'visible'
      text.style.opacity = '0'
      setTimeout(() => {
        text.style.transition = '0.5s'
        text.style.opacity = '1'
      }, 500);
    })
  }, 2);
}
function showLess() {
  const myInterval = setInterval(() => {
    document.querySelectorAll(".my-theme__item" + activ.value).forEach((element) => {
      countWidthClose.value--
      element.style.width = countWidthClose.value + 'px'
      if (countWidthClose.value < 100) {
        clearInterval(myInterval)
        countWidthClose.value = 220;
        rotateClose.value == 0
      }
    })
  }, 2);
  document.querySelectorAll(".my-theme--shape" + activ.value).forEach((shape) => {
    shape.style.transition = '0.70s'
    shape.style.transform = 'translateX(0px) rotate(0deg)'
  })
  document.querySelectorAll(".my-theme--text" + activ.value).forEach((text) => {
    text.style.visibility = 'hidden'
    text.style.transition = '0.13s'
    text.style.opacity = '0'
  })
}
showMor('', '1')
showLess()
showMor('', '1')
const count = ref(15)
setInterval(() => {
  if (count.value == 11) {
    count.value = 15
  }
  count.value--;
  document.querySelectorAll(".earth-pa").forEach((el) => [
    el.setAttribute('src', '/src/components/projectOne/assets/icon/a' + count.value + '.png')
  ])
  // console.log('yes')
}, 500);



</script>
<style scoped lang="scss">
@font-face {
  font-family: 'CustomFont';
  src: url(../../fonts/Vazir.woff2);
}

.mt-6 {
  margin-top: 130px;
}

body,
* {
  font-family: 'CustomFont';
  font-weight: normal;
  direction: rtl;
}

.my-theme {
  background-size: cover;
  background-position-x: center;
  border-radius: 30px;
  width: 100px;
  height: 300px;

  &__item1,
  &__item3 {
    background-image: url(./assets/imgs/a28.jpeg);
  }

  &__item2,
  &__item4 {
    background-image: url(./assets/imgs/a29.jpeg);
  }

  &__item5 {
    background-image: url(./assets/imgs/a30.jpeg);
  }

  &:hover {
    border: 1px solid #5681ec;
    box-shadow: 0px 7px 50px -10px rgba(115, 113, 237, 0.64);
  }
}

.shape1,
.shape2 {
  animation: translatey 5s;
  animation-iteration-count: infinite;
}

.shape3 {
  animation: translatex 8s;
  animation-iteration-count: infinite;
}

@keyframes translatey {
  0% {
    transform: translatey(0px);
  }

  50% {
    transform: translatey(80px);
  }

  100% {
    transform: translatey(0px);
  }
}

@keyframes translatex {
  0% {
    transform: translatex(0px);
  }

  25% {
    transform: translatex(-30px);
  }

  50% {
    transform: translatex(30px);
  }

  75% {
    transform: translatex(-30px);
  }

  100% {
    transform: translatex(0px);
  }
}

.mac,
.ios,
.windows,
.android {
  border: 2px solid transparent;
}

.systemsImg:hover {
  width: 50px !important;
}

.btn1 {
  height: 60px;

  &-f {
    &:hover {
      border: none;
      color: #fff;
      background-image: linear-gradient(to right, rgba(18, 168, 233, 1), rgba(115, 113, 237, 1));
    }
  }

  &-s {
    border: none;
    color: #fff;
    background-image: linear-gradient(to right, rgba(18, 168, 233, 1), rgba(115, 113, 237, 1));
  }
}

.box {
  margin-top: -130px;
  border-radius: 40px 40px 40px 40px;
  padding-right: 3rem;

  &-data {
    opacity: 0px;
    background: rgba(255, 255, 255, 0.69);
    box-shadow: 0px 4px 50px 0px rgba(115, 113, 237, 0.1);
    backdrop-filter: blur(5px);
  }
}

.earth {
  &-text {
    text-align: justify;
  }

  &-items {
    &-1 {
      margin-top: -200px;
      margin-right: -320px;
    }

    &-2 {
      margin-top: -150px;
      margin-right: -180px;
    }

    &-3 {
      margin-top: -30px;
      margin-right: 90px;
    }

    &-4 {
      margin-top: -200px;
      margin-right: 250px;
    }
  }
}

@media only screen and (max-width: 700px) {
  .earth {
    &-text {
      text-align: justify;
    }

    &-img {
      width: 350px !important;
    }

    &-items {
      &-1 {
        width: 80px !important;
        margin-top: -300px;
        margin-right: 200px;
      }

      &-2 {
        width: 80px !important;
        margin-top: -30px;
        margin-right: 20px;
      }

      &-3 {
        width: 80px !important;
        margin-top: -30px;
        margin-right: 130px;
      }

      &-4 {
        width: 80px !important;
        margin-top: -80px;
        margin-right: -30px;
      }
    }
  }
}

.sec4 {
  p {
    text-align: justify;
  }

  h4 {
    font-size: 72px;
    background: -webkit-linear-gradient(0deg, #12A9E9 0.17%, #7371ED 66.43%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }
}

.sec5 {
  @media only screen and (max-width: 700px) {
    &-img{
      width: 80% !important;
    }
  }
  background: linear-gradient(0deg, #fff, #12A9E9, #7371ED 66.43%, #fff);

  &-background {
    background: rgba(255, 255, 255, 0.842);
  }

  h6 {
    font-size: 15px;
    background: -webkit-linear-gradient(0deg, #12A9E9 0.17%, #7371ED 66.43%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }
}
</style>
