<script>

export default {
    data() {
        return {
            footerColumns: [
                {
                    title: 'DC COMICS',
                    links: [
                        'Characters',
                        'Comics',
                        'Movies',
                        'TV',
                        'Games',
                        'Videos',
                        'News'
                    ]
                },
                {
                    title: 'SHOP',
                    links: [
                        'Shop DC',
                        'Shop DC Collectibles'
                    ]
                },
                {
                    title: 'DC',
                    links: [
                        'Terms of Use',
                        'Privacy policy (New)',
                        'Ad Choices',
                        'Advertising',
                        'Jobs',
                        'Subscriptions',
                        'Talent Workshops',
                        'CPSC Certificates',
                        'Ratings',
                        'Shop Help',
                        'Contact Us'
                    ]
                },
                {
                    title: 'SITES',
                    links: [
                        'DC',
                        'MAD Magazine',
                        'DC Kids',
                        'DC Universe',
                        'DC Power Visa'
                    ]
                }
            ]

        }
    }
}

</script>

<template>
    <div id="footer-background">
        <div id="footer-container">
            <div id="footer-links">

                <div v-for="column in footerColumns" class="footer-link">
                    <strong>{{ column.title }}</strong>
                    <ul>
                        <li v-for="link in column.links">{{ link }}</li>
                    </ul>
                </div>

            </div>
            <div id="footer-logo">
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
#footer-background {
    height: 250px;
    background-image: url('/img/footer-bg.jpg');
    background-size: cover;
    background-position: center;

    #footer-container {
        height: 100%;
        max-width: 1000px;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;
        color: white;

        #footer-links {
            height: 100%;
            display: flex;
            flex-direction: column;
            flex-wrap: wrap;
            padding-top: 20px;

            .footer-link {
                padding: 5px 10px;

                ul {
                    padding: 1em 0;
                    color: #959595;
                    font-size: 0.8em;
                }
            }
        }

        #footer-logo {
            height: 100%;
            width: 350px;
            background-image: url('/img/dc-logo-bg.png');
            background-size: 350px;
            background-position: center;
        }
    }
}
</style>