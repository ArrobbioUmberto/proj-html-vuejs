<script>
export default {

}
</script>
<template>
    <div class="container">
        <span class="right-arrow">&RightArrow;</span>
        <span class="left-arrow">&leftarrow;</span>
        <h1 class="title-bg">testimonials.</h1>
        <div class="row">
            <div class="col">
                <div class="card">
                    <img src="/img/h3-img-04.png" alt="">
                    <h2 class="name">cynthia clark</h2>
                    <p class="text">"Lorem ipsum dolor sit amet consectetur adipisicing elit. Nobis quasi expedita
                        reiciendis
                        asperiores
                        repellat quam."
                    </p>
                    <div class="page-set">
                        <span class="page-number">01</span>
                        <div class="line-group">
                            <span class="white-line"></span>
                            <span class="grey-line"></span>
                        </div>
                        <span class="page-number">03</span>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../style/partials/variables.scss' as *;

.title-bg {
    color: $dark-title;
    font-size: 13.7rem;
    text-transform: capitalize;
    text-align: center;
    margin: 0;
}

.container {
    position: relative;
}

.row {
    max-width: 1380px;
    margin: 0 auto;
}

.col {
    display: flex;
    justify-content: center;
    flex-direction: row;
}

.card {
    display: flex;
    width: 50%;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    margin-top: -90px;
    padding-bottom: 90px;
}

.card>img {
    border: 4px solid $white;
    border-radius: 100%;
}

.name {
    color: $white;
    text-transform: capitalize;
}

.text {
    color: $white;
    font-weight: lighter;
    font-family: $light-font;
    font-size: 1.5rem;
}

.page-set {
    display: flex;
    flex-direction: row;
    align-items: center;
    padding: 20px 0;
}

.line-group {
    display: flex;
    padding: 0 10px;
}

.white-line {
    background-color: $white;
    height: 2px;
    width: 30px;
}

.grey-line {
    background-color: $grey-line;
    height: 2px;
    width: 60px;
}

.page-number {
    color: white;
    font-family: $light-font;
    font-weight: lighter;
}

.left-arrow,
.right-arrow {
    font-size: 2.5rem;
    color: $white;
}

.left-arrow {
    position: absolute;
    left: 0;
    top: 50%;
    transform: translate(-50%);
}

.right-arrow {
    position: absolute;
    right: 0;
    top: 50%;
    transform: translate(-50%);
}
</style>