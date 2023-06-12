<template>
    <div>
        <span 
            class="dots red-dot me-2"
            :class="{'small-dot': isSmall.small}"
        ></span>   
        <span 
            class="dots yellow-dot me-2"
            :class="{'small-dot': isSmall.small}"
        ></span>   
        <span 
            class="dots green-dot"
            :class="{'small-dot': isSmall.small}"
        ></span>   
    </div>
</template>

<script setup>
const isSmall = defineProps({
    small: {
        type: Boolean,
        default: false
    }
})
</script>

<style scoped>
.dots{
    padding: 1px;
    width: 20px;
    height: 20px;
    background-color: black;
    border-radius: 50%;
    display: inline-block;
}
.dots.small-dot{
    width: 15px;
    height: 15px;
}

.dots.red-dot{
    background-color: #FF605C;
}
.dots.yellow-dot{
    background-color: #FFBD44;
}
.dots.green-dot{
    background-color: #00CA4E;
}
</style>