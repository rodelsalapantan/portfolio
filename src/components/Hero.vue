<template>
    <div class="mb-5">
        <div class="d-flex justify-content-between mt-4 align-items-center">
            <div data-aos="fade-right">
                <img src="@/assets/img/logo.png" alt="deldev" width="90" height="90">
            </div>
            <div class="d-flex" data-aos="fade-right">
                <Socials />
            </div>

        </div>

        <div class="row" id="hero-main">
            <div class="col-md my-auto">
                <h1 id="header-name" data-aos="fade-right" data-aos-delay="100">Rodel Chris Salapantan</h1>
                <p data-aos="fade-right" data-aos-delay="300">Web Developer</p>
                <p data-aos="fade-right" data-aos-delay="500">
                    From simple HTML design, I have honed my skills to tackle complex webpages, exemplifying my commitment
                    to
                    professional growth and proficiency in the field. Highly proficient in PHP (Laravel) and Javascript.
                </p>
                <a 
                    class="btn btn-primary mt-5 px-3 py-2 d-flex align-items-center" 
                    href="mailto:rodelsalapantan@gmail.com" 
                    style="max-width: max-content;"
                    data-aos="fade-right" 
                    data-aos-delay="700"
                >
                    <i class="bi bi-chat-dots me-2"></i>
                    <span>Let's Talk!</span>
                </a>
            </div>
            <div class="col-md my-auto d-none d-lg-flex hero-images">
                <img 
                    src="@/assets/img/hero-image-left.png" 
                    alt="img" 
                    class="clipped hero-img-left"
                    data-aos="fade-up" 
                    data-aos-delay="700"
                >
                <img 
                    src="@/assets/img/hero-image-center.png" 
                    alt="img"
                    class="clipped hero-img-center"
                    data-aos="fade-up" 
                    data-aos-delay="900"
                >
                <img src="@/assets/img/hero-image-right.png" 
                    alt="" 
                    class="clipped hero-img-right"
                    data-aos="fade-up" 
                    data-aos-delay="1100"
                >

            </div>
        </div>
    </div>
</template>
<script setup>
import Socials from '@/components/partials/Socials.vue';


</script>
<style scoped>


#hero-main {
    height: 70vh;
}

#header-name{
    font-size: 40px;
}

.clipped {
    /* clip-path: polygon(25% 0%, 100% 0%, 75% 100%, 0% 100%); */
    clip-path: polygon(35% 0%, 80% 0%, 55% 100%, 10% 100%);
    cursor: pointer;
    transition: transform .2s ease-in-out;
}
.clipped:hover {
    transform: scale(1.1);
}


.hero-img-left {
    height: 350px;
    margin-left: 12px;
    margin-top: -75px;
}

.hero-img-center {
    height: 380px;
    margin-left: -210px;
}

.hero-img-right {
    height: 350px;
    margin-left: -175px;
    margin-top: -50px;
}

.hero-images::after {
    content: "";
    position: absolute;
    bottom: 90px;
    background: rgba(141, 141, 141, 0.503);
    width: 25rem;
    height: 50px;
    border-radius: 50%;
    filter: blur(20px);
    margin-left: 6rem;
}

</style>
