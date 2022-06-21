<template>
    <div>
        <nav class="navbar navbar-expand-lg">
            <div class="container">
                
                <!-- Logo -->
                <a class="navbar-brand" href="#">
                    <img src="../assets/img/dc-logo.png" alt="Nav logo" width="60">
                </a>

                <!-- Menu items -->
                <div>
                    <ul class="navbar-nav">
                        <li class="nav-item" v-for="(link, i) in navLinks" :key="i">
                            <a class="nav-link text-uppercase" :class="{active: i === 1}" href="#">{{ link.name }}</a>
                        </li>
                    </ul>
                </div>

            </div>
        </nav>
    </div>
</template>

<!-- ------------------------ -->

<script>

export default {
    name: "TheHeader",
    data() {
        return {
            navLinks: [
                {
                    name: "Characters",
                    href: "#"
                },
                {
                    name: "Comics",
                    href: "#"
                },
                {
                    name: "Movies",
                    href: "#"
                },
                {
                    name: "TV",
                    href: "#"
                },
                {
                    name: "Games",
                    href: "#"
                },
                {
                    name: "Collectibles",
                    href: "#"
                },
                {
                    name: "Videos",
                    href: "#"
                },
                {
                    name: "Fans",
                    href: "#"
                },
                {
                    name: "News",
                    href: "#"
                },
                {
                    name: "Shop",
                    href: "#"
                },
            ]
        }
    },
}

</script>

<!-- ------------------------ -->

<style lang="scss" scoped>

    

</style>