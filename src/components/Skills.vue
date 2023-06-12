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
        img: '/src/assets/img/tech_logo/laravel_noword.png',
    },
    {
        title: 'PHP',
        img: '/src/assets/img/tech_logo/php.png',
    }
    ,
    {
        title: 'C\#',
        img: '/src/assets/img/tech_logo/cs.png',
    },
    {
        title: 'MySQL',
        img: '/src/assets/img/tech_logo/mysql.png',
    },
    {
        title: 'WinForms',
        img: '/src/assets/img/tech_logo/wf.png',
    },
    {
        title: 'EF',
        img: '/src/assets/img/tech_logo/ef.png',
    },
]

const frontend = [
    {
        title: 'JavaScript',
        img: '/src/assets/img/tech_logo/js.png',
    },
    {
        title: 'jQuery',
        img: '/src/assets/img/tech_logo/jquery.png',
    }
    ,
    {
        title: 'Vue',
        img: '/src/assets/img/tech_logo/vue.png',
    },
    {
        title: 'Bootstrap',
        img: '/src/assets/img/tech_logo/bs.svg',
    },
    {
        title: 'SweetAlert',
        img: '/src/assets/img/tech_logo/swal-donut.png',
    },
    {
        title: 'HTML',
        img: '/src/assets/img/tech_logo/html.png',
    },
    {
        title: 'CSS',
        img: '/src/assets/img/tech_logo/css.png',
    }
]

const others = [
    {
        title: 'Github',
        img: '/src/assets/img/tech_logo/github.png',
    },
    {
        title: 'Pusher  ',
        img: '/src/assets/img/tech_logo/pusher-p.png',
    }
    ,
    {
        title: 'Canva',
        img: '/src/assets/img/tech_logo/canva.png',
    },
    {
        title: 'InfinityFree',
        img: '/src/assets/img/tech_logo/infinityfree.png',
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