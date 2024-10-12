<script>
export default {
    data () {
        return {
            select1: false,
            select2: false,
            selected: 'ИП Крестовоздвиженский'
        }
    }
}
</script>

<template>
    <header class="header">
        <div class="container header__container">
            <router-link to="/">
                <img :src="this.$getImage('logo.svg')" alt="">
            </router-link>
            <div class="header__right">
                <div 
                    v-click-outside="() => {select1 = false}"
                    class="header__select select"
                    :class="{
                        'active': select1
                    }"
                >
                    <button @click="select1 = !select1" class="header__select_btn">
                        <span>{{ selected }}</span>
                        <img :src="this.$getImage('corder-down.svg')" alt="">
                    </button>
                    <ul class="select_list">
                        <li v-for="i in 5" :key="i">
                            <button @click="select1 = false; selected = 'select ' + i"> select {{ i }}</button>
                        </li>
                    </ul>
                </div>
                <div class="alert">
                    <h3>24</h3>
                    <div>
                        <h4>часа</h4>
                        <p>до окончания подписки</p>
                    </div>
                </div>
                <div
                    v-click-outside="() => {select2 = false}"
                    class="header__account select"
                    :class="{
                        'active': select2
                    }"
                >
                    <button @click="select2 = !select2" class="header__account_btn">
                        <img :src="this.$getImage('user.svg')" alt="">
                        <img :src="this.$getImage('arrow-down.svg')" alt="">
                    </button>
                    <ul class="select_list">
                        <li v-for="i in 5" :key="i">
                            <a href="#"> select {{ i }}</a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </header>
</template>