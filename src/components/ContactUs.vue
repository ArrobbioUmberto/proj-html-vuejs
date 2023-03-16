<script>
export default {
    data() {
        return {
            ListBrand: [
                {
                    image: '/img/h4-clients-img-03.png',
                    red_image: '/img/h4-clients-img-04-1.png',
                    black_image: '/img/h4-clients-img-03.png'
                },
                {
                    image: '/img/h4-clients-img-05.png',
                    red_image: '/img/h4-clients-img-06-1.png',
                    black_image: '/img/h4-clients-img-05.png'
                },
                {
                    image: '/img/h4-clients-img-07.png',
                    red_image: '/img/h4-clients-img-08-1.png',
                    black_image: '/img/h4-clients-img-07.png'
                },
                {
                    image: '/img/h4-clients-img-09.png',
                    red_image: '/img/h4-clients-img-10-1.png',
                    black_image: '/img/h4-clients-img-09.png'
                },
                {
                    image: '/img/h4-clients-img-01.png',
                    red_image: '/img/h4-clients-img-02.png',
                    black_image: '/img/h4-clients-img-01.png'
                },
            ]
        }
    },
    methods: {
        ImgHover(index) {
            const red_image = this.ListBrand[index].red_image
            this.ListBrand[index].image = red_image
        },
        LeaveMouse(index) {
            const black_image = this.ListBrand[index].black_image
            this.ListBrand[index].image = black_image
        }

    }
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
                    <div class="col-50 contact_us">
                        <div class="pointer-title">
                            <h1>contact us</h1>
                            <span class="point">.</span>
                        </div>
                        <h3>Lorem ipsum dolor sit amet consectetur adipisicing elit.</h3>
                        <span class="line"></span>
                        <div class="form">
                            <div class="form_up">
                                <input type="text" placeholder="Your Name" class="name ">
                                <input type="text" placeholder="Your Email" class="mail">
                            </div>

                            <input type="text" placeholder="Write a message..." class="text">
                        </div>
                        <button class="btn">
                            <span>send </span>
                            <span class="arrow">| &rightarrow;</span>
                        </button>
                    </div>
                </div>
            </div>
            <div class="col brands">
                <ul>
                    <li v-for="(el, index) in ListBrand">
                        <img :src="el.image" v-on:mouseover="ImgHover(index)" v-on:mouseleave="LeaveMouse(index)" alt="">
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../style/partials/variables.scss' as *;

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
    row-gap: 80px;
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
    bottom: 25%;
    right: 19%;
}

.contact_us {
    display: flex;
    flex-direction: column;
    align-items: start;
}

.pointer-title {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: baseline;
}

.point {
    color: $orange-primary;
    font-size: 3rem;
}

h1 {
    text-transform: capitalize;
    margin: 0;
}

h3 {
    font-weight: lighter;
    font-weight: lighter;
    font-family: $light-font;
    font-size: 24px;
    margin: 10px 0;
}

.line {
    border-bottom: 2px solid $orange-primary;
    display: inline-block;
    width: 16%;
}

.form {
    display: flex;
    flex-wrap: wrap;
    padding: 20px 0;
    justify-content: space-between;
}

.form_up {
    display: flex;
    flex-basis: 100%;
    gap: 20px;
    flex-direction: row;
}

input {
    border: none;
}

input:focus {
    outline: none;
}

.text,
.mail,
.name {
    border-bottom: 1px solid $variant-black;
    padding-left: 10px;
    text-align: start;
}

.name,
.mail {
    flex-basis: 50%;
}

.text {
    width: 100%;
    height: 100px;
    flex-grow: 1;

}

.btn>span {
    padding: 0 17px;
    font-weight: bold;
}

.btn {
    background-color: $orange-primary;
    border: none;
    text-transform: uppercase;
    padding: 14px 10px;
    color: white;
    margin-top: 20px;
    display: flex;
    align-items: baseline;
}

span.arrow {
    font-size: 25px;
    font-weight: lighter;
    font-family: $light-font;
    line-height: 30px;

}

.brands {
    padding: 20px 0;
}

ul {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
}

li {
    list-style-type: none;
}
</style>