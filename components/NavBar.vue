<template>
    <nav class="navbar navbar-expand-lg">
        <div class="container-xxl d-flex justify-content-between">
            <a class="navbar-brand m-0 p-0 d-flex" href="#">
                <img src="/images/logo.svg" alt="">
            </a>
            <ul class="navbar-nav mb-2 mb-lg-0 d-none d-lg-flex li-gap">
                <li class="nav-item">
                    <a class="nav-link" aria-current="page" href="#">Home</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">About Us</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">Services</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">Project</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">Contact Us</a>
                </li>
            </ul>
            <a href="#" class="get-started-btn btn d-none d-lg-block">
                Get Started
            </a>
            <button class="navbar-toggler" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasNavbar" aria-controls="offcanvasNavbar" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="offcanvas offcanvas-end d-block d-lg-none" tabindex="-1" id="offcanvasNavbar" aria-labelledby="offcanvasNavbarLabel">
                <div class="offcanvas-header">
                    <a class="navbar-brand p-0 d-flex" href="#">
                        <img src="/images/logo.svg" alt="">
                    </a>
                    <button type="button" class="btn-close" data-bs-dismiss="offcanvas" aria-label="Close"></button>
                </div>
                <div class="offcanvas-body">
                    <ul class="navbar-nav justify-content-end flex-grow-1 li-gap">
                        <li class="nav-item">
                            <a class="nav-link" aria-current="page" href="#">Home</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">About Us</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Services</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Project</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Contact Us</a>
                        </li>
                        <li>
                            <a href="#" class="get-started-btn btn w-100">
                                Get Started
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </nav>
</template>
<script>
export default {
    
}
</script>
<style lang="scss" scoped>

    @import "~/assets/scss/mixins/breakpoints";

    .navbar {
        padding: 16px 0;
    }

    @include media-breakpoint-up(lg) {
        .navbar {
            padding-top: 24px;
        }
    }

    .nav-link {
        color: #1E1E1E;
        font-family: Open Sans;
        font-size: 15px;
        font-style: normal;
        font-weight: 500;
        line-height: normal;

        &:hover {
            text-decoration: underline;
        }
    }

    .li-gap {
        gap: 20px 40px;
    }

    .get-started-btn {
        border-radius: 5px;
        background: #0E1017;

        color: #FFF;
        text-align: center;
        font-family: Open Sans;
        font-size: 20px;
        font-style: normal;
        font-weight: 600;
        line-height: 120%; /* 24px */

        padding: 16px 24px;
    }
</style>