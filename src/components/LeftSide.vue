<template>
    <div class="promo relative py-16 pl-32 h-screen text-white" style="border-radius: 0 100px 100px 0 ">
        <div class="logo flex">
            <img src="../assets/images/logo.svg" alt="travel agency logo">
            <div class="ml-5 text-xl font-semibold">Travel<span class="font-light">.app</span></div>
        </div>
        <div class="bottom absolute left-0" style="padding: inherit; top: 50%">
            <h1 class="font-bold text-6xl" style="line-height: 64px">The Whole World <br>
            in One Place</h1>
            <h2 class="mt-8 font-light text-lg" style="line-height: 29px">Discover the most unique places, experiences<br>
                and amazing homes around the world.</h2>
            <button class="mt-8 py-5 w-44 text-base rounded-xl" style="background-color: #8BB957">Sign Up</button>
            <div class="slider flex mt-16 items-center">
                <div class="relative" style="">
                    <div class="slider__dots-line mr-12"></div>
                    <div class="slider__dot absolute top-0 left-0 "></div>
                </div>
                <div class="slider__counter font-light text-lg">
                    <span class="font-bold">01</span> &ndash; 05
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'LeftSide'
}
</script>
    
<style scoped>
    .promo {
        background-image: url('../assets/images/bg-1.png');
        background: linear-gradient(270deg, transparent 50%, rgba(0, 0, 0, 0.7) 100%), url('../assets/images/bg-1.png') no-repeat top/cover;
    }
    .slider__dots-line {
        width: 260px;
        height: 2px;
        background: #FFFFFF;
        opacity: 0.3;
        border-radius: 1px;
    }
    .slider__dot {
        width: 30%;
        height: 2px;
        background: white;
        transition: 1s all;
        border-radius: 1px;
    }
</style>