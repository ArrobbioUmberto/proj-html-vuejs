<script>
export default {

}
</script>
<template>
    <div class="container">
        <div class="row wrap">
            <div class="col">
                <div class="row up-section">
                    <div class="col-50 map">
                        <img src="/img/h1-contact-rev-01.png" alt="">
                        <img src="/img/h1-contact-rev-02.png" alt="" class="plus-1">
                        <img src="/img/h1-contact-rev-02.png" alt="" class="plus-2">
                        <img src="/img/h1-contact-rev-02.png" alt="" class="plus-3">

                    </div>
                    <div class="col-50">form</div>
                </div>
            </div>
            <div class="col"> brand li</div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.container {
    padding: 100px 0;
}

.row {
    max-width: 1380px;
    margin: 0 auto;
}

.wrap {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

.up-section {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
}

.col {
    width: 100%;
    text-align: center;
}

.col-50 {
    flex-basis: 50%;
}

.map {
    position: relative;
}

.plus-1 {
    position: absolute;
    top: 37%;
    left: 27%;
}

.plus-2 {
    position: absolute;
    top: 21%;
    left: 50%;
}

.plus-3 {
    position: absolute;
    bottom: 20%;
    right: 19%;
}
</style>