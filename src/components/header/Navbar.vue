<script >
export default {
    data() {
        return {
            Menulist: [
                { text: 'homes' },
                { text: 'pages' },
                { text: 'blog' },
                { text: 'shop' },
                { text: 'events' },
                { text: 'elements' }
            ]
        }

    }
}
</script>

<template>
    <div class="container header">
        <div class="row">
            <div class="col">
                <img src="/img/logo-img-01.png" alt="logo">
            </div>
            <div class="col">
                <ul class="nav_menu">
                    <li><a href="#" class="arrow">&rightarrow;</a></li>
                    <li v-for="el in Menulist">
                        <a href="#">{{ el.text }}</a>
                    </li>
                    <li><a href=""><i class="fa-solid fa-magnifying-glass"></i></a></li>
                    <li><a href=""><i class="fa-solid fa-list"></i></a></li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../../style/partials/variables.scss' as *;

.header {
    height: 100px;
}

.nav_menu {
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    align-items: center;
}

.row {
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-direction: row;
    padding: 30px 0;
}

a {
    text-decoration: none;
    text-transform: uppercase;
    margin: 5px 10px;
    font-weight: bold;
    color: $normal-text;
    padding: 10px 0;
}

li {
    list-style-type: none;
    margin: 0 10px;
}

.arrow {
    font-size: 24px;
    margin: 0 -20px;
    padding: 0 10px;
}

a:hover {
    color: $primary;
    cursor: pointer;
}
</style>