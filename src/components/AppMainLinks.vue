<script>

export default {
    data() {
        return {
            mainLinks: [
                {
                    imageLink: '/img/buy-comics-digital-comics.png',
                    nameLink: 'DIGITAL COMICS'
                },
                {
                    imageLink: '/img/buy-comics-merchandise.png',
                    nameLink: 'DC MERCHANDISE'
                },
                {
                    imageLink: '/img/buy-comics-subscriptions.png',
                    nameLink: 'SUBSCRIPTION'
                },
                {
                    imageLink: '/img/buy-comics-shop-locator.png',
                    nameLink: 'COMIC SHOP LOCATOR'
                },
                {
                    imageLink: '/img/buy-dc-power-visa.svg',
                    nameLink: 'DC POWER VISA'
                },
            ]
        };
    },
}
</script>

<template>
    <div id="container-main-links">
        <div id="main-links">
            <div v-for="link in mainLinks" class="link">
                <img :src="link.imageLink" alt="">
                <div>{{ link.nameLink }}</div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
#container-main-links {
    height: 100px;
    display: flex;
    align-items: center;
    background-color: #0282f9;


    #main-links {
        width: 1000px;
        margin: 0 auto;
        display: flex;
        justify-content: space-around;
        align-items: center;

        .link {
            display: flex;
            align-items: center;
            gap: 10px;
            color: white;

            img {
                height: 32px;
            }
        }
    }
}
</style>