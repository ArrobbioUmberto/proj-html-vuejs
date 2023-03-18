<script>
export default {
    data() {
        return {
            PhotoList: [
                {
                    image: '/img/h1-img-01.jpg'
                },
                {
                    image: '/img/h1-img-02.jpg'
                },
                {
                    image: '/img/h1-img-03.jpg'
                },
            ],
            currentIndex: 0,
        }
    },
    methods: {
        previousImage() {
            const lastIndex = this.PhotoList.length - 1
            if (this.currentIndex === 0) {
                this.currentIndex = lastIndex
            } else {
                this.currentIndex--
            }
        },
        nextImage() {
            if (this.currentIndex === this.PhotoList.length - 1) {
                this.currentIndex = 0
            } else {
                this.currentIndex++
            }
        }
    }
}
</script>
<template>
    <div class="container">
        <div class="row">
            <div v-for="(el, index) in PhotoList" class="col-img" :class="{ hidden: index != currentIndex }">
                <div class="card-img">
                    <img :src="el.image" alt="">
                    <div class="arrow-box">
                        <span @click="previousImage" class="left-arrow">&leftarrow;</span>
                        <span @click="nextImage" class="right-arrow">&RightArrow;</span>
                    </div>

                </div>
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
        </div>
        <img src="/svg/svg-4.svg" alt="" class="point-circle">
    </div>
</template>
<style lang="scss" scoped>
@use '../../style/partials/variables.scss' as *;

.container {
    position: relative;

}

.hidden {
    display: none;
}

.left-arrow,
.right-arrow {
    font-size: 2rem;
    color: $white;
    margin: 0 5px;
}

.arrow-box {
    background-color: $orange-primary;
    max-width: max-content;
    position: absolute;
    bottom: 4px;
    padding: 20px 30px;
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
    background-color: $orange-primary;
    padding: 10px 20px;
    color: $white;
    margin-bottom: 4px;
}

.col-text {
    background-color: $white;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(0%, -50%);
    padding: 130px 50px;
    z-index: 1;
}

.line {
    border-bottom: 2px solid $orange-primary;
    display: inline-block;
    width: 16%;
}

.description {
    font-weight: 300;
    font-family: $light-font;
    line-height: 25px;
}

h2 {
    font-size: 35px;
    text-transform: capitalize;
    margin: 0;
}

h3 {
    font-weight: 300;
    font-family: $light-font;
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
    background-color: $orange-primary;
    color: $white;
    aspect-ratio: 1/1;
    border-radius: 25px;
    padding: 5px;
    margin: 0 5px;
}

.fb {
    padding: 5px 8px;
}

.immagine {
    background-color: $black;
}
</style>