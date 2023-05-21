<template>
    <nav class="nav">
        <div class="container">
            <div class="nav__box">
                <h2 class="logo"><a href="#">{{ logo }}</a></h2>
                <ul class="nav__list">
                    <li v-for="(item, i) in navLinks" :key="i"><a href="#" class="nav__link">{{ item }}</a></li>

                </ul>
            </div>
        </div>
    </nav>
</template>

<script>
    export default {

        props: {
            navLinks: {
                type: Array
            },
            logo: {
                type: String
            }
        }
        
    }
</script>

<style>

</style>