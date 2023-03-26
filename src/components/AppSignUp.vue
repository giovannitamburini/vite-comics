<script>
export default {
    data() {
        return {
            socialImages: [
                '/img/footer-facebook.png',
                '/img/footer-twitter.png',
                '/img/footer-youtube.png',
                '/img/footer-pinterest.png',
                '/img/footer-periscope.png',
            ]
        }
    }
}
</script>

<template>
    <div id="signup-background">
        <div id="signup-container">
            <button>SIGN-UP NOW!</button>
            <div id="social-container">
                <div id="follow">FOLLOW US</div>
                <div v-for="socialImage in socialImages" class="social">
                    <img :src="socialImage" alt="">
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
#signup-background {
    height: 80px;
    background-color: #303030;

    #signup-container {
        width: 1000px;
        height: 100%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;

        button {
            padding: 9px;
            color: white;
            background-color: transparent;
            border: 2px solid #0282f9;
            cursor: pointer;
        }

        #social-container {
            display: flex;
            align-items: center;
            gap: 12px;

            #follow {
                color: #0282f9;
                font-size: 1.1em;
                font-weight: 700;
            }

            .social {
                img {
                    height: 25px;
                }
            }


        }
    }
}
</style>