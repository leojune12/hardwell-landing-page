<template>
    <div class="pt-5">
        <div class="footer-section py-5">
            <div class="container-xxl pt-5">
                <div class="row text-center gy-5 gy-md-0">
                    <div class="col-md-3 wd-logo d-flex align-items-center justify-content-center justify-content-md-start">
                        WD
                    </div>
                    <div class="col-md-3 d-flex flex-column">
                        <div class="category mb-3">
                            Menu
                        </div>
                        <div class="mb-2">
                            <a href="#" class="link">
                                About
                            </a>
                        </div>
                        <div class="mb-2">
                            <a href="#" class="link mb-2">
                                Portfolio
                            </a>
                        </div>
                        <div class="mb-2">
                            <a href="#" class="link mb-2">
                                Blog
                            </a>
                        </div>
                        <div class="mb-2">
                            <a href="#" class="link">
                                Contact
                            </a>
                        </div>
                    </div>
                    <div class="col-md-3 d-flex flex-column">
                        <div class="category mb-3">
                            Service
                        </div>
                        <div class="mb-2">
                            <a href="#" class="link mb-2">
                                User Experience
                            </a>
                        </div>
                        <div class="mb-2">
                            <a href="#" class="link mb-2">
                                User Interface
                            </a>
                        </div>
                        <div class="mb-2">
                            <a href="#" class="link mb-2">
                                Logotype
                            </a>
                        </div>
                        <div class="mb-2">
                            <a href="#" class="link">
                                See More
                            </a>
                        </div>
                    </div>
                    <div class="col-md-3 social-links d-flex gap-3 align-items-center justify-content-center justify-content-md-end">
                        <a href="#" class="d-flex justify-content-center align-items-center">
                            <img src="/images/icons8-facebook.svg" alt="">
                        </a>
                        <a href="#" class="d-flex justify-content-center align-items-center">
                            <img src="/images/icons8-twitter.svg" alt="">
                        </a>
                        <a href="#" class="d-flex justify-content-center align-items-center">
                            <img src="/images/icons8-instagram.svg" alt="">
                        </a>
                    </div>
                </div>
                <div class="d-flex flex-column flex-md-row justify-content-between pt-5 row-gap-3">
                    <div class="copyright-text text-center">
                        Copyright © 2020 Laaqiq. All Rights Reserved.
                    </div>
                    <div class="text-center">
                        <a href="#" class="link me-5">
                            Terms of Use
                        </a>
                        <a href="#" class="link">
                            Privacy Policy
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style lang="scss" scoped>
    .footer-section {
        background: #111;

        .wd-logo {
            color: #FFF;
            font-family: Epilogue;
            font-size: 40px;
            font-style: normal;
            font-weight: 700;
            line-height: 48px; /* 120% */
        }

        .category {
            color: rgba(255, 255, 255, 0.50);
            font-family: Epilogue;
            font-size: 16px;
            font-style: normal;
            font-weight: 400;
            line-height: 32px; /* 200% */
            letter-spacing: 3px;
            text-transform: uppercase;
        }

        .link {
            color: #FFF;
            font-family: Epilogue;
            font-size: 16px;
            font-style: normal;
            font-weight: 400;
            line-height: 32px; /* 200% */
            text-decoration: none;

            &:hover {
                text-decoration: underline;
            }
        }

        .social-links {
            a {
                width: 44px;
                height: 44px;
                background: #242424;
                border-radius: 100%;
            }
        }

        .copyright-text {
            color: rgba(255, 255, 255, 0.50);
            font-family: Epilogue;
            font-size: 16px;
            font-style: normal;
            font-weight: 400;
            line-height: 32px; /* 200% */
        }
    }
</style>