<script>
export default {

}
</script>
<template>
    <div class="container">
        <div class="row">
            <div class="col-img">
                <img src="/img/h1-img-01.jpg" alt="">
                <span class="arrow">&leftarrow;&rightarrow;</span>

            </div>
            <div class="col-text">
                <h2>jason bickford</h2>
                <h3>Founder and Executive Director</h3>
                <span>linea </span>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Eveniet totam rem consectetur incidunt,
                    provident vero vel? Excepturi, qui nemo.</p>
            </div>
        </div>
        <img src="/svg/svg-4.svg" alt="" class="point-circle">
    </div>
</template>
<style lang="scss" scoped>
.container {
    position: relative;
}

.row {
    display: flex;
    flex-direction: row;
    position: relative;
    justify-content: space-between;
    padding: 30px 0;
    max-width: 1380px;
    margin: 0 auto;
}

.col-img {
    position: relative;
}

.arrow {
    position: absolute;
    bottom: 0;
    left: 0;
    font-size: 30px;
    background-color: #ff4612;
    padding: 10px 20px;
    color: white;
}

.col-text {
    background-color: white;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(0%, -50%);
    padding: 80px 50px;
    z-index: 1;
}

h2 {
    font-size: 35px;
    text-transform: capitalize;
}

.point-circle {
    position: absolute;
    top: 0;
    right: 0%;
}
</style>