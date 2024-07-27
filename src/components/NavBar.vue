<template>
    <nav class="navbar navbar-expand-lg bg-body-tertiary">
        <div class="container-fluid p-0 px-3">
            <a class="navbar-brand" href="#"><img src="../assets/icon/shape1.png" alt=""></a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
                data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false"
                aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                    <li class="nav-item">
                        <a class="nav-link" aria-current="page" href="#">assets</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">why to buy crypto</a>
                    </li>
                    <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown"
                        aria-expanded="false">
                        how it works
                    </a>
                    <ul class="dropdown-menu w-100 p-3" >
                        <div class="w-100 row">
                            <div class="col-6 d-flex">
                                <div>
                                    <img class="dropdown-menu--img" src="../assets/icon/createAcont.png" alt="">
                                </div>
                                <div class="ps-2">
                                    <h2 class="dropdown-menu--title">create an account</h2>
                                    <p class="dropdown-menu--description">Lorem ipsum dolor sit amet, consectetur
                                        adipiscing elit</p>
                                </div>
                            </div>
                            <div class="col-6 d-flex">
                                <div>
                                    <img class="dropdown-menu--img" src="../assets/icon/blueacont.png" alt="">
                                </div>
                                <div class="ps-2">
                                    <h2 class="dropdown-menu--title">create an account</h2>
                                    <p class="dropdown-menu--description">Lorem ipsum dolor sit amet, consectetur
                                        adipiscing elit</p>
                                </div>
                            </div>
                        </div>
                        <div class="w-100 row">
                            <div class="col-6 d-flex">
                                <div>
                                    <img class="dropdown-menu--img" src="../assets/icon/greenacont.png" alt="">
                                </div>
                                <div class="ps-2">
                                    <h2 class="dropdown-menu--title">create an account</h2>
                                    <p class="dropdown-menu--description">Lorem ipsum dolor sit amet, consectetur
                                        adipiscing elit</p>
                                </div>
                            </div>
                            <div class="col-6 d-flex">
                                <div>
                                    <img class="dropdown-menu--img" src="../assets/icon/orangeacont.png" alt="">
                                </div>
                                <div class="ps-2">
                                    <h2 class="dropdown-menu--title">create an account</h2>
                                    <p class="dropdown-menu--description">Lorem ipsum dolor sit amet, consectetur
                                        adipiscing elit</p>
                                </div>
                            </div>
                        </div>
                        <div class="w-100 row">
                            <div class="col-6 d-flex">
                                <div>
                                    <img class="dropdown-menu--img" src="../assets/icon/blueacont.png" alt="">
                                </div>
                                <div class="ps-2">
                                    <h2 class="dropdown-menu--title">create an account</h2>
                                    <p class="dropdown-menu--description">Lorem ipsum dolor sit amet, consectetur
                                        adipiscing elit</p>
                                </div>
                            </div>
                            <div class="col-6 d-flex">
                                <div>
                                    <img class="dropdown-menu--img" src="../assets/icon/orangeacont.png" alt="">
                                </div>
                                <div class="ps-2">
                                    <h2 class="dropdown-menu--title">create an account</h2>
                                    <p class="dropdown-menu--description">Lorem ipsum dolor sit amet, consectetur
                                        adipiscing elit</p>
                                </div>
                            </div>
                        </div>
                        <div class="w-100 row">
                            <div class="col-6 d-flex">
                                <div>
                                    <img class="dropdown-menu--img" src="../assets/icon/createAcont.png" alt="">
                                </div>
                                <div class="ps-2">
                                    <h2 class="dropdown-menu--title">create an account</h2>
                                    <p class="dropdown-menu--description">Lorem ipsum dolor sit amet, consectetur
                                        adipiscing elit</p>
                                </div>
                            </div>
                            <div class="col-6 d-flex">
                                <div>
                                    <img class="dropdown-menu--img" src="../assets/icon/greenacont.png" alt="">
                                </div>
                                <div class="ps-2">
                                    <h2 class="dropdown-menu--title">create an account</h2>
                                    <p class="dropdown-menu--description">Lorem ipsum dolor sit amet, consectetur
                                        adipiscing elit</p>
                                </div>
                            </div>
                        </div>
                    </ul>
                </ul>
            </div>
        </div>
    </nav>
</template>
<style lang="scss">
.navbar {
    background: rgba(166, 150, 209, 0.1) !important;
    color: #fff !important;
    border-radius: 999px;
    height: 60px;
    width: 686px;
    opacity: 0px;

    .nav-link {
        color: #fff;
        font-size: 17px;
    }

    .dropdown-menu {
        background: rgba(166, 150, 209, 0.1);
        backdrop-filter: blur(10px);

        color: #fff !important;
        border: none !important;
        border-radius: 0px 0px 30px 30px;

        &--img {
            width: 45px;
        }

        &--title {
            font-size: 13px;
        }

        &--description {
            font-size: 10px;
            margin-top: -7px;
        }
    }

    &:has(.show) {
        border-radius: 30px 30px 0px 0px;

        .show {
            color: #865BFF;
            border-bottom: 1px solid #865BFF;
        }
    }
}
</style>