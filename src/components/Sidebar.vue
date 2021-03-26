<template>
    <div class="nav">
        <div class="mobile-nav">
            <button class="mobile-nav__burger-button" @click="showNav">
                <font-awesome-icon icon="bars" v-if="!sidebarShow"/>
                <font-awesome-icon icon="times" v-else/>

            </button>
            <a href="#">
                <img class="mobile-nav__logo" src="../assets/img/cupup-logo-text.svg">
            </a>
            <button class="mobile-nav__alert-button">
                <font-awesome-icon icon="bell"/>
            </button>
        </div>
        <div :class="[{sidebar_show:sidebarShow},'sidebar']" >

                    <div class="sidebar__scroll-wrapper">
                        <div class="sidebar__scroll" v-bar="{
    preventParentScroll: true,
}">
                            <div>
                                <div class="sidebar__content">

                                <div class="sidebar__header">
                            <a href="#">
                                <img class="sidebar__logo" src="../assets/img/cupup-logo-text.svg">
                            </a>
                            <button class="sidebar__alert-button">
                                <font-awesome-icon icon="bell"/>
                            </button>

                            <ul class="sidebar__nav">
                                <li class="sidebar__nav-item sidebar__nav-item_active">
                                    <a href="#">
                                        <font-awesome-icon icon="user"/>
                                        Профиль
                                    </a>
                                </li>
                                <li class="sidebar__nav-item">
                                    <a href="#">
                                        <font-awesome-icon icon="users"/>
                                        Команды
                                    </a>
                                </li>
                                <li class="sidebar__nav-item">
                                    <a href="#">
                                        <font-awesome-icon icon="trophy"/>
                                        Чемпионаты
                                    </a>
                                </li>
                                <li class="sidebar__nav-item">
                                    <a href="#">
                                        <font-awesome-icon icon="trophy"/>
                                        Чемпионаты
                                    </a>
                                </li>
                                <li class="sidebar__nav-item">
                                    <a href="#">
                                        <font-awesome-icon icon="trophy"/>
                                        Чемпионаты
                                    </a>
                                </li>
                                <li class="sidebar__nav-item">
                                    <a href="#">
                                        <font-awesome-icon icon="trophy"/>
                                        Чемпионаты
                                    </a>
                                </li>
                            </ul>
                        </div>

                        <div class="sidebar__banner">
                            <button class="banner__close-button">
                                <font-awesome-icon icon="times-circle"/>
                            </button>
                            <span class="banner__text">
                Подпишись, чтобы не пропустить чемпионаты
            </span>
                            <img class="banner__image" src="../assets/img/postbox.png">
                            <button class="banner__confirm-button">Подписаться</button>
                        </div>
                    </div>
                </div>
                        </div>
            </div>
        </div>
        <div class="sidebar__tint" v-if="sidebarShow"></div>
    </div>
</template>

<script>
    export default {
        name: 'Sidebar',
        data(){
            return{
                sidebarShow:false,
            }
        },
        methods:{
            showNav(){
                this.sidebarShow = !this.sidebarShow;
                if(this.sidebarShow) {
                    document.body.style.overflow = 'hidden'
                } else{
                    document.body.style.overflow = 'auto'
                }
            }
        }
    }

</script>

<style scoped>

</style>
