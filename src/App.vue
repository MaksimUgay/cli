<template>
    <div>
        <Navbar :logo="logo" :navLinks="navLinks"></Navbar>
        <HeaderContent></HeaderContent>
        <Main></Main>
        <Footer></Footer>
    </div>
    
</template>

<script>
import Navbar from './components/Navbar.vue';
import HeaderContent from './components/HeaderContent.vue';
import Main from './components/Main.vue';
import Footer from './components/Footer.vue';

    export default {
        components: { Navbar, HeaderContent, Main, Footer },
        
        data() {
            return {
                navLinks: ['Обо мне', 'Мои работы', 'Контакты'],
                logo: 'PROWEB'
            }
        }
    }
</script>
