<template>
    <div>
    <div class="overlay first"></div>
    <div class="overlay second"></div>
    <div class="overlay third"></div>
    </div>
</template>

<style lang="scss" scoped>
    .overlay{
        position: absolute;
        width: 100%;
        height: 100%;
        top: 0;
        z-index: 99;
        overflow: hidden;
        &.first{ 
            background: #fcc419;
        }
        &.second{
            background: #fcc419;
            left: 33.33%;
        }
        &.third{
            background: #fcc419;
            left: 66.66%;
        }
    }
</style>

<script>
import {gsap} from 'gsap';
export default {
    activate() {
        gsap.to(".first", {
            duration: 1.5,
            delay: 0.5,
            top: "-100%",
            ease: "expo.inOut",
        });

        gsap.to(".second", {
            duration: 1.5,
            delay: 0.6,
            top: "-100%",
            ease: "expo.inOut",
        });

        gsap.to(".third", {
            duration: 1.5,
            delay: 0.7,
            top: "-100%",
            ease: "expo.inOut",
        });
    }   
}
</script>