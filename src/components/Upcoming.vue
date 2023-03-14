<script>
export default {

}
</script>
<template>
    <div class="container-lg event-section">
        <div class="row">
            <ul>
                <li>
                    <h1 class="row-title">upcoming events</h1>
                </li>
                <li class="text">
                    <div class="date">
                        <p class="day"> 07</p>
                        <p class="month">Jan. 2022</p>
                    </div>
                    <div class="event">
                        <h2 class="title">melbourne coaching</h2>
                        <p class="hours">
                            <i class="fa-regular fa-clock"></i>
                            <span>9:00 am - 5:00 pm, Jan 7, 2022</span>
                        </p>
                        <p class="place">
                            <i class="fa-solid fa-location-dot"></i>
                            <span>Cambridge, MA 02138, USA</span>
                        </p>
                        <button class="btn">read more</button>
                    </div>
                </li>
                <li class="text">
                    <div class="date">
                        <p class="day"> 07</p>
                        <p class="month">Jan. 2022</p>
                    </div>
                    <div class="event">
                        <h2 class="title">melbourne coaching</h2>
                        <p class="hours">
                            <i class="fa-regular fa-clock"></i>
                            <span>9:00 am - 5:00 pm, Jan 7, 2022</span>
                        </p>
                        <p class="place">
                            <i class="fa-solid fa-location-dot"></i>
                            <span>Cambridge, MA 02138, USA</span>
                        </p>
                        <button class="btn">read more</button>
                    </div>
                </li>
                <li class="text">
                    <div class="date">
                        <p class="day"> 07</p>
                        <p class="month">Jan. 2022</p>
                    </div>
                    <div class="event">
                        <h2 class="title">melbourne coaching</h2>
                        <p class="hours">
                            <i class="fa-regular fa-clock"></i>
                            <span>9:00 am - 5:00 pm, Jan 7, 2022</span>
                        </p>
                        <p class="place">
                            <i class="fa-solid fa-location-dot"></i>
                            <span>Cambridge, MA 02138, USA</span>
                        </p>
                        <button class="btn">read more</button>
                    </div>
                </li>
            </ul>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.event-section {
    max-width: 1380px;
    margin: 0 auto;
    height: 100%;
    display: flex;
    align-items: center;
}

.row {
    display: flex;
    flex-direction: column;
    background-color: white;
    max-width: 700px;
}

ul {
    padding: 0;
    margin: 0;
}

li {
    list-style-type: none;
    padding: 30px 200px 30px 40px;
    border-bottom: 1px solid rgba(0, 0, 0, 0.2);
    background-color: #fafafa;
}

li:hover {
    background-color: #ffffff;
}

.text {
    display: flex;
    flex-direction: row;
    align-items: start;
}

.row-title {
    text-transform: capitalize;
}

.date {
    color: white;
    padding: 10px;
    background-color: #ff4612;
    text-align: center;
    font-family: "Source Sans Pro", sans-serif;
    margin-top: 20px;
}

.day {
    font-weight: bold;
    margin: 0;
    font-size: 20px;
    font-family: "Source Sans Pro", sans-serif;
}

.month {
    font-weight: lighter;
    margin: 0;
}

.event {
    margin: 0 20px;
}

i {
    color: #ff4612;
    margin-right: 5px;
}

.title {
    text-transform: capitalize;
}

.hours,
.place {
    font-weight: 300;
    font-family: "Source Sans Pro", sans-serif;
    line-height: 15px;
}

.btn {
    border: none;
    background-color: transparent;
    text-transform: uppercase;
    font-weight: 600;
    font-size: 11px;
}
</style>