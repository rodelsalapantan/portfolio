<template>
    <a href="https://www.facebook.com/rodelsalapantan/">
        <i class="bi bi-facebook me-2"></i>
    </a>
    <a href="mailto:rodelsalapantan@gmail.com">
        <i class="bi bi-envelope-fill bi-rounded-fill me-2"></i>
    </a>
    <a href="https://www.linkedin.com/in/rodel-chris-salapantan-b30317154/">
        <i class="bi bi-linkedin bi-rounded-fill me-2"></i>
    </a>
    <a href="https://github.com/rodelsalapantan">
        <i class="bi bi-github bi-rounded-fill"></i>
    </a>
</template>

<style scoped>
.bi::before {
    font-size: 31px;
}

.bi.bi-rounded-fill::before {
    font-size: 17px;
    padding: 6px;
    border: 1px solid black;
    border-radius: 50%;
    background-color: black;
    color: #ffffff;
}

.bi.bi-envelope-fill::before {
    border-color: #C6483A;
    background-color: #C6483A;
}

.bi.bi-linkedin::before {
    border-color: #0A66C2;
    background-color: #0A66C2;
}

.bi.bi-github::before {
    border-color: #000000;
    background-color: #000000;
}
</style>