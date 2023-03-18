<script>
export default {

}
</script>
<template>
    <div class="container">
        <div class="row">
            <ul class="list-wrap">
                <li class="col">
                    <ul class="list-item">
                        <li class="title">about</li>
                        <li><span class="line"></span></li>
                        <li>
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing.
                                Dolore, aspernatur esse modi tempora debitis qui!
                                Laboriosam corporis, dolorum ut nobis accusamus asperiores.</p>
                        </li>
                        <li class="logo">
                            <i class="fa-brands fa-linkedin-in custom-logo"></i>
                            <i class="fa-brands fa-facebook-f custom-logo fb"></i>
                            <i class="fa-brands fa-twitter custom-logo"></i>
                        </li>
                    </ul>
                </li>
                <li class="col">
                    <ul class="list-item">
                        <li class="title">twitter</li>
                        <li><span class="line"></span></li>
                        <li class="twitter-text">
                            <i class="fa-brands fa-twitter"></i>
                            <p class="text">Lorem ipsum dolor sit amet consectetur adipisicing.
                                Dolore, aspernatur esse modi tempora debitis qui!
                                Laboriosam corporis, dolorum ut nobis accusamus asperiores.</p>
                        </li>
                        <li class="twitter-text">
                            <i class="fa-brands fa-twitter"></i>
                            <p class="text">Lorem ipsum dolor sit amet consectetur adipisicing.
                                Dolore, aspernatur esse modi tempora debitis qui!
                                Laboriosam corporis, dolorum ut nobis accusamus asperiores.</p>
                        </li>
                    </ul>
                </li>
                <li class="col">
                    <ul class="important_links list-item">
                        <li class="title">important links</li>
                        <li><span class="line"></span></li>
                        <li><a href="#">about me</a></li>
                        <li><a href="#">about us</a></li>
                        <li><a href="#">language packs</a></li>
                        <li><a href="#">become a coach</a></li>
                        <li><a href="#">monthly events</a></li>

                    </ul>
                </li>
                <li class="col">
                    <ul class="list-item">
                        <li class="title">contact me</li>
                        <li><span class="line"></span></li>
                        <li class="contact place"><i class="fa-solid fa-location-dot"></i> 457 bigblue street, NY 10013</li>
                        <li class="contact"><i class="fa-solid fa-phone"></i>(315) 5512-2579</li>
                        <li class="contact"><i class="fa-regular fa-envelope"></i>everlead@mikado.com</li>
                        <li class="form-part">
                            <input class="input-box" type="text" placeholder="Your Name">
                            <button class="btn">subscribe</button>
                        </li>
                    </ul>
                </li>
            </ul>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../../style/partials/variables.scss' as *;

.col {
    flex-basis: calc(100% / 4);
}

.row {
    padding: 90px 0;
    max-width: 1380px;
    margin: 0 auto;
}

p {
    margin: 0;
    color: $text-invert;
    font-family: $light-font;
    font-weight: lighter;
    font-size: 15px;
}

.title {
    color: $text-invert;
    font-size: 30px;
    font-weight: bold;
}

.text {
    padding: 0 10px;
}

.fa-twitter {
    color: $primary;
}

.list-wrap {
    display: flex;
    flex-direction: row;
    gap: 30px;
    padding: 40px 0;
    padding-inline-start: 0;
}

.list-item {
    padding: 0;
    display: flex;
    flex-direction: column;
    gap: 10px;
}

li {
    list-style-type: none;
}

.line {
    border-bottom: 2px solid $primary;
    display: inline-block;
    width: 10%;
}

.twitter-text {
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    padding: 10px 0;
}

.logo {
    display: flex;
    flex-direction: row;
    align-items: center;
}

.custom-logo {
    background-color: $text-invert;
    color: $normal-text;
    aspect-ratio: 1/1;
    border-radius: 25px;
    padding: 5px;
    margin: 10px 5px;
}

.custom-logo:hover {
    color: $primary;
    transform: scale(1.3);
}

.fb {
    padding: 5px 8px;
}

a {
    color: $text-invert;
    text-decoration: none;
}

.title::first-letter {
    text-transform: capitalize;
}

.important_links a {
    padding: 10px 0;
    color: $text-invert;
    font-family: $light-font;
    font-weight: lighter;
    font-size: 15px;
}

.important_links li {
    padding: 5px 0;
}

.important_links li::first-letter {
    text-transform: capitalize;
}

.contact {
    color: $text-invert;
    font-family: $light-font;
    font-weight: lighter;
    margin: 10px 0;
}

.place {
    text-transform: capitalize;
}

.contact i {
    color: $primary;
    padding: 0 5px;
}


.btn {
    background-color: transparent;
    color: $text-invert;
    border: none;
    text-transform: uppercase;
}

.form-part {
    background-color: transparent;
    border-bottom: 1px solid $text-invert;
    width: max-content;
}

.input-box {
    background-color: transparent;
    border: none;
    padding: 10px 0;
    color: $text-invert;
}

input:focus {
    outline: none;
}
</style>