<script >
export default {

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
                    <li><a href=""></a>homes</li>
                    <li><a href=""></a>pages</li>
                    <li><a href=""></a>blog</li>
                    <li><a href=""></a>shop</li>
                    <li><a href=""></a>events</li>
                    <li><a href=""></a>elements</li>
                    <li><a href=""></a><i class="fa-solid fa-magnifying-glass"></i></li>
                    <li><a href=""></a><i class="fa-solid fa-list"></i></li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.header {
    height: 100px;
}

.nav_menu {
    display: flex;
    flex-direction: row;
    justify-content: space-around;
}

.row {
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-direction: row;
    padding: 30px 0;
}

li {
    list-style-type: none;
    text-transform: uppercase;
    margin: 5px 10px;
    font-weight: bold;
}

li:hover {
    color: orange;
    cursor: pointer;
}
</style>