<template>
    <button class="post-btn">ACCEDER</button>
</template>

<script setup>

</script>

<style scoped>
.post-btn{
    width: 205px;
    height: 80px;
    cursor: pointer ;
    color: #fff;
    font-size: 24px;
    border-radius: 16px;
    border: none;
    outline: none;
    position: relative;
    background-color: black;
    text-transform: uppercase;
}

.post-btn::after{
    content: '';
    width: 100%;
    height: 100%;
    background: radial-gradient(
        circle farthest-corner at 10% 20%,
        rgba(255,94,274,1) 18%,
        rgba(2,245,255,1) 100%
    );
    filter: blur(15px);
    position: absolute;
    left: 0;
    top: 0;
    z-index: -1;
    animation: move 2s linear infinite;
    background-size:40% 200% 
}

.post-btn:hover{
    background-color: black;

}

@keyframes move {
    0%{
        background-position: 0 0;
    }
    100%{
        background-position: 200px 440px;
    }
}
</style>


