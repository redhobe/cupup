<template>
    <div class="sidebar">
            <div v-bar="{
    preventParentScroll: true,
}">                <div>
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
</template>

<script>
    export default {
        name: 'Sidebar',
    }

</script>

<style scoped>

</style>
