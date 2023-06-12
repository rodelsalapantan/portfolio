<template>
    <div class="mt-big border-top">
        <div class="footer py-2 px-4 mt-5">
            <div class="row mb-5">
                <div class="col-lg mb-5 mb-lg-0 text-center text-lg-start">
                    <h1
                        data-aos="fade-right" 
                        data-aos-duration="1000"
                        data-aos-delay="200"
                    >Get in Touch</h1>
                    <p 
                        class="desc mb-5 w-lg-50"
                        data-aos="fade-right" 
                        data-aos-duration="1000"
                        data-aos-delay="400"
                    >Have a suggestion or want to share your thoughts? I'm all ears. <br />
                        Contact me today!
                    </p>
                    <a 
                        href="mailto:rodelsalapantan@gmail.com"
                        class="btn btn-outline-dark msg-now-btn rounded-1 py-2"
                        data-aos="fade-right" 
                        data-aos-duration="1000"
                        data-aos-delay="600"
                        >Message Now!</a>
                </div>
                <div 
                    class="col-lg d-flex flex-column justify-content-center text-center"
                    data-aos="fade-left" 
                    data-aos-duration="1000"
                    data-aos-delay="800"
                >
                    <p>Social Links:</p>
                    <div class="d-flex justify-content-center">
                        <Socials />
                    </div>
                </div>
            </div>

        </div>

        <div class="footer-banner">
            <p class="mb-0 p-4">Made by: Rodel Chris Salapantan</p>
            <a 
                href="#top-contact" 
                class="floating-btn text-decoration-none"
                data-aos="fade-up" 
                data-aos-duration="1000"
                data-aos-delay="1000"
            >
                <i class="bi bi-arrow-bar-up"></i>
                <p class="small text-secondary">Back to Top</p>
            </a>
        </div>
    </div>
</template>

<script setup>
import Socials from '@/components/partials/Socials.vue';
</script>

<style scoped>
.footer,
.footer-banner>p {
    max-width: 1280px;
    margin: 0 auto;
}

.desc {
    color: #707070;
}

.msg-now-btn {
    width: 15rem;
}

.footer-banner {
    background-color: #111827;
    color: #6B6B6B;
    position: relative;
}

a.floating-btn {
    position: absolute;
    top: -150%;
    right: 20px;
    text-align: center;
}

a.floating-btn > .bi.bi-arrow-bar-up::before {
    font-size: 35px;
    color: white;
    padding: 10px;
    border-radius: 50%;
    border: 1px solid #707070;

    background-color: #707070;

}
</style>