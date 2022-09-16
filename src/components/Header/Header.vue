<script setup>
// Style
import styles from './Header.module.css'

// Icons
import star from "../../assets/icons/star.png";
import searchIcon from "../../assets/icons/searchIcon.png";
import avatarIcon from "../../assets/icons/avatarIcon.png";
import cartIcon from "../../assets/icons/cartIcon.png";
</script>

<template>
    <header :class="styles.headerContainer">
        <div :class="styles.headerLeft">
            <img :class="styles.star" :src="star" alt="star" />
            <h3 :class="styles.headerTitle">selfcare</h3>
        </div>
        <nav :class="styles.headerRight">
            <img :class="styles.searchIcon" :src="searchIcon" alt="search" />
            <img :class="styles.avatarIcon" :src="avatarIcon" alt="avatar" />
            <img :class="styles.cartIcon" :src="cartIcon" alt="cart" />
        </nav>
    </header>
</template>