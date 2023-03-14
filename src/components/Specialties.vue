<script>
export default {

}
</script>
<template>
    <div class="container circle">
        <div class=" row row-text">
            <div class="pointer-title">
                <h1>our specialities</h1>
                <span class="point">.</span>
            </div>
            <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.</p>
            <span class="line"></span>
        </div>
        <div class="row row-card">
            <ul>
                <li>
                    <img src="/svg/svg-0.svg" alt="">
                    <h2>knowing</h2>
                    <p>Lorem ipsum, dolor sit amet consectetur adipisicing.</p>
                </li>
                <li>
                    <img src="/svg/svg-1.svg" alt="">
                    <h2>knowing</h2>
                    <p>Lorem ipsum, dolor sit amet consectetur adipisicing.</p>
                </li>
                <li>
                    <img src="/svg/svg-2.svg" alt="">
                    <h2>knowing</h2>
                    <p>Lorem ipsum, dolor sit amet consectetur adipisicing.</p>
                </li>
                <li>
                    <img src="/svg/svg-3.svg" alt="">
                    <h2>knowing</h2>
                    <p>Lorem ipsum, dolor sit amet consectetur adipisicing.</p>
                </li>
            </ul>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.container.circle {
    background-color: white;
    position: relative;
    top: -150px;
}

.row {
    max-width: 1380px;
    margin: 0 auto;
}

.row-text {
    text-align: center;
}

.pointer-title {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: baseline;
}

.point {
    color: #ff4612;
    font-size: 6rem;
}

h1 {
    font-size: 45px;
    text-transform: capitalize;
    margin: 0;
}

p {
    font-weight: lighter;
    font-family: 'Source Sans Pro', sans-serif;
    font-size: 24px;
    margin: 0;
}

.row-card {
    padding: 70px 0;
}

ul {
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    align-items: center;
}

li {
    list-style-type: none;
    text-align: center;
}

h2 {
    text-transform: capitalize;
}

.line {
    border-bottom: 2px solid #ff4612;
    display: inline-block;
    width: 6%;
}
</style>