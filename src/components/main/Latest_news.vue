<script>
export default {
    data() {
        return {
            Cardlist: [
                {
                    image: '/img/h1-blog-img-02.jpg',
                    title: 'boost motivation',
                    time_event: 'May 5, 2019',
                    speaker: 'amanda doe',
                    btn: 'read more',
                    text: 'Lorem, ipsum dolor sit amet consectetur adipisicing elit. Repellendus quae obcaecati nihil repudiandae....'
                },
                {
                    image: '/img/h1-blog-img-03.jpg',
                    title: 'team building',
                    time_event: 'May 5, 2019',
                    speaker: 'amanda doe',
                    btn: 'read more',
                    text: 'Lorem, ipsum dolor sit amet consectetur adipisicing elit. Repellendus quae obcaecati nihil repudiandae....'
                },
                {
                    image: '/img/h1-blog-img-04.jpg',
                    title: 'next investment',
                    time_event: 'May 5, 2019',
                    speaker: 'amanda doe',
                    btn: 'read more',
                    text: 'Lorem, ipsum dolor sit amet consectetur adipisicing elit. Repellendus quae obcaecati nihil repudiandae....'
                },
                {
                    image: '/img/h1-blog-img-01.jpg',
                    title: 'new business day',
                    time_event: 'May 5, 2019',
                    speaker: 'amanda doe',
                    btn: 'read more',
                    text: 'Lorem, ipsum dolor sit amet consectetur adipisicing elit. Repellendus quae obcaecati nihil repudiandae....'
                }

            ],
        }

    },
    methods: {

    }
}
</script>
<template>
    <div class="container">
        <img src="/svg/svg-4.svg" alt="" class="point-circle">
        <div class=" row row-text">
            <div class="pointer-title">
                <h1>latest news</h1>
                <span class="point">.</span>
            </div>
            <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.</p>
            <span class="line"></span>
        </div>
        <div class="row row-card">
            <div class="col">
                <div v-for="(el, index) in Cardlist" class="card">
                    <div class="card-img">
                        <img :src="el.image" alt="">
                        <button class="btn-corner"><i class="fa-solid fa-tag"></i>business, leading</button>
                    </div>
                    <div class="event-info">
                        <span class="date"> <i class="fa-regular fa-clock"></i> {{ el.time_event }}</span>
                        <span class="speaker"><i class="fa-regular fa-user"></i> {{ el.speaker }}</span>
                    </div>
                    <h2>{{ el.title }}</h2>
                    <p class="card-text">{{ el.text }}</p>
                    <button class="btn">{{ el.btn }}</button>
                </div>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../../style/partials/variables.scss' as *;

.container {
    position: relative;
    padding: 100px 0;
}

.row {
    max-width: 1380px;
    margin: 0 auto;
    overflow: auto;
}

.row-text {
    text-align: center;
    padding: 40px 0;
}

.point-circle {
    position: absolute;
    top: -100px;
    left: 0;
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
    font-size: 45px;
    text-transform: capitalize;
    margin: 0;
}

p {
    font-weight: lighter;
    font-family: $light-font;
    font-size: 24px;
    margin: 0;
}

.line {
    border-bottom: 2px solid $orange-primary;
    display: inline-block;
    width: 6%;
}

.col {
    display: flex;
    flex-direction: row;
    gap: 40px;
    padding: 0;
    overflow: auto;
}

.card {
    display: flex;
    flex-direction: column;
    flex-basis: calc((100% / 3) - 39px);
    flex-grow: 0;
    flex-shrink: 0;
    position: relative;
}

.col::-webkit-scrollbar {
    height: 10px;
}

.row-card>.col::-webkit-scrollbar-thumb {
    border-radius: 25px;
    background-color: $orange-primary;
}


.event-info {
    padding-top: 40px;
}

.date,
.speaker {
    font-weight: lighter;
    font-family: $light-font;
    font-size: 1rem;
    padding: 0 5px;
    text-transform: capitalize;
}

h2 {
    margin: 0;
    padding: 10px 0;
    text-transform: capitalize;
}

i {
    color: $orange-primary;
}

.btn-corner>i {
    color: $white;
    padding: 0 3px;
}

.card-text {
    font-size: 1rem;
    line-height: 1.5rem;
    font-weight: lighter;
}

.card-img>img {
    width: 100%;
    z-index: 1;
}

.btn-corner {
    background-color: $orange-primary;
    width: max-content;
    border: none;
    text-transform: capitalize;
    padding: 10px;
    color: $white;
    position: absolute;
    right: 5%;
    bottom: 40%;
    padding: 1rem 1.5rem;
    font-weight: lighter;
    font-family: $light-font;
}

.btn {
    width: fit-content;
    border: none;
    font-weight: bolder;
    font-size: 0.9rem;
    text-transform: uppercase;
    background-color: transparent;
    padding: 15px 0;
}

.left-arrow,
.right-arrow {
    font-size: 2.5rem;
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