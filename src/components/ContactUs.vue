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
                        <button class="btn"> <span>send </span> <span class="arrow">| &rightarrow;</span> </button>
                    </div>
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
    color: #ff4612;
    font-size: 3rem;
}

h1 {
    text-transform: capitalize;
    margin: 0;
}

h3 {
    font-weight: lighter;
    font-weight: lighter;
    font-family: 'Source Sans Pro', sans-serif;
    font-size: 24px;
    margin: 10px 0;
}

.line {
    border-bottom: 2px solid #ff4612;
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

input:active {
    border: none;
}

.text,
.mail,
.name {
    border-bottom: 1px solid rgba(0, 0, 0, 0.3);
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
    background-color: #ff4612;
    border: none;
    text-transform: uppercase;
    padding: 10px;
    color: white;
    margin-top: 20px;
    display: flex;
    align-items: baseline;
}

span.arrow {
    font-size: 25px;
    font-weight: lighter;
    font-family: 'Source Sans Pro', sans-serif;
    line-height: 30px;

}
</style>