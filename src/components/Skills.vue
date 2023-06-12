<template>
    <div class="skills-container mb-big">
        <div class="top text-center mb-5">
            <h1 
                data-aos="fade-left" 
                data-aos-duration="1000"
            >Skills</h1>
            <p 
                class="subtitle mb-3"
                data-aos="fade-left" 
                data-aos-duration="1000"
                data-aos-delay="200"
            >My Technical Competencies</p>
        </div>
        <div class="row gx-4 gy-3 gy-lg-0">
            <div class="col-lg-4">
                <div 
                    class="card shadowbox" 
                    data-aos="fade-up" 
                    data-aos-duration="1000"
                    data-aos-delay="400">
                    <div class="border-bottom p-2 pb-1">
                        <ThreeDots small />
                    </div>
                    <div>
                        <div class="title p-4">
                            <h3><i class="bi bi-stack me-4"></i>BACKEND</h3>
                        </div>
                        <div class="container text-center">
                            <div class="row row-cols-3">
                                <div class="col" v-for="item in backend">
                                    <div>
                                        <img :src="item.img" alt="img" height="45">
                                    </div>
                                    <div>
                                        <p>{{ item.title }}</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <div class="col-lg-4">
                <div 
                    class="card shadowbox"
                    data-aos="fade-up" 
                    data-aos-duration="1000"
                    data-aos-delay="600"
                    >
                    <div class="border-bottom p-2 pb-1">
                        <ThreeDots small />
                    </div>
                    <div>
                        <div class="title p-4">
                            <h3><i class="bi bi-code-slash me-4"></i>FRONTEND</h3>
                        </div>
                        <div class="container text-center">
                            <div class="row row-cols-3">
                                <div class="col" v-for="item in frontend">
                                    <div>
                                        <img :src="item.img" alt="img" height="45">
                                    </div>
                                    <div>
                                        <p>{{ item.title }}</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <div class="col-lg-4">
                <div 
                    class="card shadowbox"
                    data-aos="fade-up" 
                    data-aos-duration="1000"
                    data-aos-delay="800"
                >
                    <div class="border-bottom p-2 pb-1">
                        <ThreeDots small />
                    </div>
                    <div>
                        <div class="title p-4">
                            <h3><i class="bi bi-lightbulb me-4"></i>OTHERS</h3>
                        </div>
                        <div class="container text-center">
                            <div class="row row-cols-3">
                                <div class="col" v-for="item in others">
                                    <div>
                                        <img :src="item.img" alt="img" height="45">
                                    </div>
                                    <div>
                                        <p>{{ item.title }}</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </div>
</template>

<script setup>
import ThreeDots from '@/components/partials/ThreeDots.vue';


const backend = [
    {
        title: 'Laravel',
        img: new URL('@/assets/img/tech_logo/laravel_noword.png', import.meta.url),
    },
    {
        title: 'PHP',
        img: new URL('@/assets/img/tech_logo/php.png', import.meta.url),
    }
    ,
    {
        title: 'C\#',
        img: new URL('@/assets/img/tech_logo/cs.png', import.meta.url),
    },
    {
        title: 'MySQL',
        img: new URL('@/assets/img/tech_logo/mysql.png', import.meta.url),
    },
    {
        title: 'WinForms',
        img: new URL('@/assets/img/tech_logo/wf.png', import.meta.url),
    },
    {
        title: 'EF',
        img: new URL('@/assets/img/tech_logo/ef.png', import.meta.url),
    },
]

const frontend = [
    {
        title: 'JavaScript',
        img: new URL('@/assets/img/tech_logo/js.png', import.meta.url),
    },
    {
        title: 'jQuery',
        img: new URL('@/assets/img/tech_logo/jquery.png', import.meta.url),
    }
    ,
    {
        title: 'Vue',
        img: new URL('@/assets/img/tech_logo/vue.png', import.meta.url),
    },
    {
        title: 'Bootstrap',
        img: new URL('@/assets/img/tech_logo/bs.svg', import.meta.url),
    },
    {
        title: 'SweetAlert',
        img: new URL('@/assets/img/tech_logo/swal-donut.png', import.meta.url),
    },
    {
        title: 'HTML',
        img: new URL('@/assets/img/tech_logo/html.png', import.meta.url),
    },
    {
        title: 'CSS',
        img: new URL('@/assets/img/tech_logo/css.png', import.meta.url),
    }
]

const others = [
    {
        title: 'Github',
        img: new URL('@/assets/img/tech_logo/github.png', import.meta.url),
    },
    {
        title: 'Pusher  ',
        img: new URL('@/assets/img/tech_logo/pusher-p.png', import.meta.url),
    }
    ,
    {
        title: 'Canva',
        img: new URL('@/assets/img/tech_logo/canva.png', import.meta.url),
    },
    {
        title: 'InfinityFree',
        img: new URL('@/assets/img/tech_logo/infinityfree.png', import.meta.url),
    },
]

</script>

<style scoped>
.skills-container {
    margin-top: 10rem;
    height: 100%;
}

.bi::before {
    font-size: 1.75rem;
}

.card.shadowbox {
    min-height: 24rem;
}
</style>