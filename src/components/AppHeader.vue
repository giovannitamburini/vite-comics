<script>

export default {
    data() {
        return {
            navLinks: [
                'CHARACTERS',
                'COMICS',
                'MOVIES',
                'TV',
                'GAMES',
                'COLLECTIBLES',
                'VIDEOS',
                'FANS',
                'NEWS',
                'SHOP'
            ]
        }
    }
}
</script>

<template>
    <div id="nav-container">
        <nav>
            <div id="logo">
                <img src="/img/dc-logo.png" alt="dc logo">
            </div>

            <div id="nav-links">
                <ul>
                    <li v-for="navLink in navLinks">{{ navLink }}</li>
                </ul>
            </div>

        </nav>

    </div>
</template>

<style lang="scss" scoped>
#nav-container {
    width: 100%;
    height: 80px;
    background-color: #ffffff;
    display: flex;
    justify-content: center;

    nav {
        width: 1000px;
        height: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;

        #logo {

            img {
                height: 60px;
            }
        }

        #nav-links {
            ul {
                display: flex;
                flex-flow: row nowrap;
                justify-content: center;
                align-items: stretch;
                gap: 20px;

                li {

                    font-weight: bold;
                    position: relative;
                    cursor: pointer;

                    &:hover {
                        color: #0282f9;
                    }

                    &:hover::before {
                        content: '';
                        position: absolute;
                        width: 100%;
                        height: 5px;
                        bottom: -31px;
                        background-color: #0282f9;
                    }
                }
            }
        }
    }
}
</style>