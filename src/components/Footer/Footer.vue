<script setup>
// Style
import styles from './Footer.module.css'

// Icons
import instaIcon from "../../assets/icons/instaIcon.png";
import faceIcon from "../../assets/icons/faceIcon.png";
import masterIcon from "../../assets/icons/masterIcon.png";
import payIcon from "../../assets/icons/payIcon.png";
import visaIcon from "../../assets/icons/visaIcon.png";
</script>

<template>
    <footer :class="styles.footerContainer">
        <div :class="styles.footerContent">
            <div :class="styles.links">
                <ul>
                    <li><a href="#">Contato</a></li>
                    <li><a href="#">Termos de serviço</a></li>
                    <li><a href="#">Política de privacidade</a></li>
                    <li><a href="#">Cancelamento, troca e reembolso</a></li>
                </ul>
            </div>
            <div :class="styles.newsletter">
                <h3>Newsletter</h3>
                <form>
                    <input type="email" placeholder="Digite seu melhor e-mail" />
                    <button><span>Inscrever</span></button>
                </form>
            </div>
            <div :class="styles.socialAndPayment">
                <div :class="styles.social">
                    <a href="#"><img :class="styles.instaIcon" :src="instaIcon" alt="instagram" /></a>
                    <a href=""><img :class="styles.faceIcon" :src="faceIcon" alt="facebook" /></a>
                </div>
                <div :class="styles.payment">
                    <img :class="styles.masterIcon" :src="masterIcon" alt="mastercard" />
                    <img :class="styles.payIcon" :src="payIcon" alt="paypal" />
                    <img :class="styles.visaIcon" :src="visaIcon" alt="visa" />
                </div>
            </div>
        </div>
    </footer>
</template>