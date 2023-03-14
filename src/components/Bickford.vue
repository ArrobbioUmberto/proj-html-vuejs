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
                <span class="line"></span>
                <p class="description">Lorem ipsum dolor sit amet consectetur adipisicing elit. Eveniet totam rem
                    consectetur incidunt,
                    provident vero vel? Excepturi, qui nemo.</p>
                <div class="sign-section">
                    <div class="logo">
                        <i class="fa-brands fa-linkedin-in custom-logo"></i>
                        <i class="fa-brands fa-facebook-f custom-logo fb"></i>
                        <i class="fa-brands fa-twitter custom-logo"></i>
                    </div>
                    <img src="/img/firma.png" alt="" class="sign">
                </div>
            </div>
            <!-- <img src="/svg/svg-5.svg" alt="logo circolare grande"> -->
            <!-- <img src="/svg/svg-6.svg" alt="freccia" class="immagine"> -->
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
    margin-bottom: 4px;
}

.col-text {
    background-color: white;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(0%, -50%);
    padding: 130px 50px;
    z-index: 1;
}

.line {
    border-bottom: 2px solid #ff4612;
    display: inline-block;
    width: 16%;
}

.description {
    font-weight: 300;
    font-family: "Source Sans Pro", sans-serif;
    line-height: 25px;
}

h2 {
    font-size: 35px;
    text-transform: capitalize;
    margin: 0;
}

h3 {
    font-weight: 300;
    font-family: "Source Sans Pro", sans-serif;
    font-size: 20px;
    margin: 0;
}

.point-circle {
    position: absolute;
    top: 0;
    right: 0%;
}

.sign-section {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
}

.sign {
    margin-right: 30%;
}

.logo {
    display: flex;
    flex-direction: row;
    align-items: center;
}

.custom-logo {
    background-color: #ff4612;
    color: white;
    aspect-ratio: 1/1;
    border-radius: 25px;
    padding: 5px;
    margin: 0 5px;
}

.fb {
    padding: 5px 8px;
}

.immagine {
    background-color: black;
}
</style>