<script setup>
// Styles
import styles from './Main.module.css'

// Images
import banner from "../../assets/images/banner.png";

// Components
import Products from '../../helpers/Products.vue';
</script>

<template>
    <main :class="styles.mainContainer">
        <div :class="styles.bannerContainer">
            <img :src="banner" alt="banner" />
        </div>
        <div :class="styles.mainTitles">
            <div :class="styles.title01">
                <h3>promoção</h3>
            </div>
            <div :class="styles.title02">
                <h3>9 produtos</h3>
            </div>
        </div>
        <div :class="styles.mainContent">
            <Products />
        </div>
    </main>
</template>