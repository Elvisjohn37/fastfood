<template>
    <div :class="styles.mainNavigation">
        <ion-menu content-id="main-content">
            <ion-content class="ion-padding"
                ><div :class="styles.sideMenu">
                    <div :class="styles.profile">
                        <div :class="styles.image">
                            <div :class="styles.avatar">
                                <img
                                    src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT80lmS918O4AJ-A197bvSjLY9CTHZNmyi4AA&usqp=CAU"
                                />
                            </div>
                            <div :class="styles.icon">
                                <font-awesome-icon :icon="faCrown" />
                            </div>
                            <div :class="styles.points">
                                0 Points<font-awesome-icon
                                    :class="styles.arrow"
                                    :icon="faGreaterThan"
                                />
                            </div>
                        </div>
                        <div :class="styles.info">
                            <div :class="styles.name">Chou Tzuyu</div>
                            <div :class="styles.number">09111111111</div>
                        </div>
                    </div>
                    <div :class="styles.menus">
                        <ul>
                            <li>
                                <IonNavLink to="/"
                                    ><font-awesome-icon
                                        :class="[styles.menuIcon, styles.active]"
                                        :icon="faHome"
                                    />Home</IonNavLink
                                >
                            </li>
                            <li>
                                <IonNavLink to="/ordernow"
                                    ><font-awesome-icon
                                        :class="styles.menuIcon"
                                        :icon="faDrumstickBite"
                                    />Order Now!</IonNavLink
                                >
                            </li>
                            <li>
                                <IonNavLink to="/"
                                    ><font-awesome-icon
                                        :class="styles.menuIcon"
                                        :icon="faDrumstickBite"
                                    />Notifications</IonNavLink
                                >
                            </li>
                            <li>
                                <IonNavLink to="/"
                                    ><font-awesome-icon
                                        :class="styles.menuIcon"
                                        :icon="faDrumstickBite"
                                    />Store Locator</IonNavLink
                                >
                            </li>
                            <li>
                                <IonNavLink to="/"
                                    ><font-awesome-icon
                                        :class="styles.menuIcon"
                                        :icon="faDrumstickBite"
                                    />FAQ's</IonNavLink
                                >
                            </li>
                            <hr />
                            <li>
                                <IonNavLink to="/"
                                    ><font-awesome-icon
                                        :class="styles.menuIcon"
                                        :icon="faDrumstickBite"
                                    />My Orders</IonNavLink
                                >
                            </li>
                            <li>
                                <IonNavLink to="/"
                                    ><font-awesome-icon
                                        :class="styles.menuIcon"
                                        :icon="faDrumstickBite"
                                    />My Account</IonNavLink
                                >
                            </li>
                            <li>
                                <IonNavLink to="/"
                                    ><font-awesome-icon
                                        :class="styles.menuIcon"
                                        :icon="faDrumstickBite"
                                    />My Favorites</IonNavLink
                                >
                            </li>
                            <li>
                                <IonNavLink to="/"
                                    ><font-awesome-icon
                                        :class="styles.menuIcon"
                                        :icon="faDrumstickBite"
                                    />Order Tracker</IonNavLink
                                >
                            </li>
                            <li>
                                <IonNavLink to="/"
                                    ><font-awesome-icon
                                        :class="styles.menuIcon"
                                        :icon="faDrumstickBite"
                                    />Order History</IonNavLink
                                >
                            </li>
                            <li>
                                <ion-button
                                    expand="block"
                                    :class="styles.logout"
                                    >Logout</ion-button
                                >
                            </li>
                        </ul>
                    </div>
                </div></ion-content
            >
        </ion-menu>
        <ion-page id="main-content">
            <ion-header>
                <ion-toolbar>
                    <ion-buttons slot="start">
                        <ion-menu-button></ion-menu-button>
                    </ion-buttons>
                    <ion-title>Loyalty Points</ion-title>
                </ion-toolbar>
            </ion-header>
            <ion-content class="ion-padding">
                Tap the button in the toolbar to open the menu.
            </ion-content>
        </ion-page>
    </div>
</template>

<script setup>
import styles from './MainNavigation.module.scss'
import { IonNavLink } from '@ionic/vue'
import {
    faCrown,
    faGreaterThan,
    faHome,
    faDrumstickBite,
} from '@fortawesome/free-solid-svg-icons'
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
import {
    IonButtons,
    IonContent,
    IonHeader,
    IonMenu,
    IonMenuButton,
    IonPage,
    IonTitle,
    IonToolbar,
    IonButton,
} from '@ionic/vue'
</script>
