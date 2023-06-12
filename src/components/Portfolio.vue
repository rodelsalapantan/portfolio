<template>
    <div class="py-5" data-aos="fade" data-aos-duration="2000">
        <ThreeDots />
    </div>
    <div class="text-center mb-big" data-aos="fade-up" >
        <h1 id="header-name">Portfolio</h1>
        <p class="subtitle">Recent Projects</p>
    </div>
    <div class="container mb-big">
        <div 
            v-for="(item, index) in cardDetails" 
            :key="index" 
            class="row mb-big card-container flex-nowrap"
            data-aos="fade-up" 
            data-aos-duration="2000"
        >
            <div
                class="shadowbox col-12 col-lg-3 d-flex flex-column border rounded left-card me-4 col-offset-2 py-4 px-3 align-items-center justify-content-center">
                <div class="mb-4">
                    <img :src="item.project_logo" alt="img" width="100">
                </div>
                <h5 class="mb-4 text-center fw-bold">{{ item.title }}</h5>
                <div class="mb-4 text-center">
                    <img v-for="(logo, logo_index) in item.tech_stack_logo" :key="logo_index" :src="logo" alt="img"
                        height="25" class="me-2">
                </div>
                <a 
                    :href="item.link"
                    class="btn btn-outline-primary w-100"
                    target="_blank"
                >View <i class="bi bi-caret-right-fill"></i>
                </a>
            </div>
            <div class="shadowbox d-none d-lg-block col-lg-9 right-card border rounded left-card p-0 overflow-hidden">
                <div class="border-bottom p-2 pb-0">
                    <ThreeDots small />
                </div>
                <div class="container text-center p-3 align-items-center">
                    <div class="row row-cols-2 gy-4">
                        <div v-for="(screenshot, index) in item.screenshots" :key="index" class="col">
                            <img class="image-showcase" :src="screenshot" alt="img">
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import ThreeDots from './partials/ThreeDots.vue';

const cardDetails = [
    {
        // 1
        title: 'EC - E-Commerce and IT-related services',
        project_logo: new URL('@/assets/img/portfolio/1/logo.png', import.meta.url),
        tech_stack_logo: [
            new URL('@/assets/img/tech_logo/php.png', import.meta.url),
            new URL('@/assets/img/tech_logo/bs.svg', import.meta.url),
            new URL('@/assets/img/tech_logo/jquery.png', import.meta.url),
            new URL('@/assets/img/tech_logo/pusher.png', import.meta.url),
            new URL('@/assets/img/tech_logo/swal.png', import.meta.url),
        ],
        screenshots: [
            new URL('@/assets/img/portfolio/1/1.png', import.meta.url),
            new URL('@/assets/img/portfolio/1/2.png', import.meta.url),
            new URL('@/assets/img/portfolio/1/3.png', import.meta.url),
            new URL('@/assets/img/portfolio/1/4.png', import.meta.url),
        ],
        link: 'http://eccapstone.epizy.com/',
    },
    {
        // 2 
        title: 'Online Movie Downloader App',
        project_logo: new URL('@/assets/img/portfolio/2/logo.png', import.meta.url),
        tech_stack_logo: [
            new URL('@/assets/img/tech_logo/wf.png', import.meta.url),
            new URL('@/assets/img/tech_logo/cs.png', import.meta.url),
        ],
        screenshots: [
            new URL('@/assets/img/portfolio/2/1.png', import.meta.url),
            new URL('@/assets/img/portfolio/2/2.png', import.meta.url),
            new URL('@/assets/img/portfolio/2/3.png', import.meta.url),
            new URL('@/assets/img/portfolio/2/4.png', import.meta.url),
        ],
        link: 'https://github.com/rodelsalapantan/movie-collection-app',
    },
    {
        // 3
        title: 'Quiz Generator App',
        project_logo: new URL('@/assets/img/portfolio/3/logo.png', import.meta.url),
        tech_stack_logo: [
            new URL('@/assets/img/tech_logo/laravel.png', import.meta.url),
        ],
        screenshots: [
            new URL('@/assets/img/portfolio/3/1.png', import.meta.url),
            new URL('@/assets/img/portfolio/3/2.png', import.meta.url),
            new URL('@/assets/img/portfolio/3/3.png', import.meta.url),
            new URL('@/assets/img/portfolio/3/4.png', import.meta.url),
        ],
        link: 'https://github.com/rodelsalapantan/Laravel_QuizGeneratorApp/',
    },
    {
        // 4
        title: 'Grades Viewer App',
        project_logo: new URL('@/assets/img/portfolio/4/logo.png', import.meta.url),
        tech_stack_logo: [
            new URL('@/assets/img/tech_logo/laravel.png', import.meta.url),
        ],
        screenshots: [
            new URL('@/assets/img/portfolio/4/1.png', import.meta.url),
            new URL('@/assets/img/portfolio/4/2.png', import.meta.url),
            new URL('@/assets/img/portfolio/4/3.png', import.meta.url),
            new URL('@/assets/img/portfolio/4/4.png', import.meta.url),
        ],
        link: 'https://github.com/rodelsalapantan/grades-viewer-app',
    },
    {
        // 5
        title: 'Faina\'s Site',
        project_logo: new URL('@/assets/img/portfolio/5/logo.png', import.meta.url),
        tech_stack_logo: [
            new URL('@/assets/img/tech_logo/canva.png', import.meta.url),
        ],
        screenshots: [
            new URL('@/assets/img/portfolio/5/1.png', import.meta.url),
            new URL('@/assets/img/portfolio/5/2.png', import.meta.url),
            new URL('@/assets/img/portfolio/5/3.png', import.meta.url),
            new URL('@/assets/img/portfolio/5/4.png', import.meta.url),
        ],
        link: 'https://fainas.my.canva.site',
    },
    {
        // 6
        title: 'Host Miriam Site',
        project_logo: new URL('@/assets/img/portfolio/1/logo.png', import.meta.url),
        tech_stack_logo: [
            new URL('@/assets/img/tech_logo/canva.png', import.meta.url),
        ],
        screenshots: [
            new URL('@/assets/img/portfolio/6/1.png', import.meta.url),
            new URL('@/assets/img/portfolio/6/2.png', import.meta.url),
            new URL('@/assets/img/portfolio/6/3.png', import.meta.url),
            new URL('@/assets/img/portfolio/6/4.png', import.meta.url),
        ],
        link: '#',
    },

]

</script>

<style scoped>
.left-card, .right-card {
    height: 25rem;
    
}

.image-showcase {
    max-width: 100%;
    max-height: 150px;
    transition: transform .2s ease-in-out;
}

.image-showcase:hover {
    transform: scale(1.1);
}
</style>