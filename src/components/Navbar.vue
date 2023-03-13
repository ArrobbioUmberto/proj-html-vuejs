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
                    <li><a href=""> &rightarrow; homes</a></li>
                    <li><a href="">pages</a></li>
                    <li><a href="">blog</a></li>
                    <li><a href="">shop</a></li>
                    <li><a href="">events</a></li>
                    <li><a href="">elements</a></li>
                    <li><a href=""><i class="fa-solid fa-magnifying-glass"></i></a></li>
                    <li><a href=""><i class="fa-solid fa-list"></i></a></li>
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
    color: black;
    padding: 10px 0;
}

li {
    list-style-type: none;
    margin: 0 10px;

}

a:hover {
    color: orange;
    cursor: pointer;
}
</style>