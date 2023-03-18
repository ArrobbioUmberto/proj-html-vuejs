<script>
export default {
    data() {
        return {
            Listevents: [
                {
                    day: '7',
                    month: 'jan. 2022',
                    title: 'melbourne coaching',
                    time_event: '9:00 am - 5:00 pm, Jan 7, 2022',
                    place: 'Cambridge, MA 02138, USA',
                    btn: 'read more'
                },
                {
                    day: '11',
                    month: 'jan. 2022',
                    title: 'new york coaching',
                    time_event: '9:00 am - 5:00 pm, Jan 11, 2022',
                    place: 'Cambridge, MA 02138, USA',
                    btn: 'read more'
                },
                {
                    day: '21',
                    month: 'jan. 2022',
                    title: 'london coaching',
                    time_event: '9:00 am - 5:00 pm, Jan 21, 2022',
                    place: 'Cambridge, MA 02138, USA',
                    btn: 'read more'
                },
            ]
        }
    }
}
</script>
<template>
    <div class="container-lg event-section">
        <div class="row">
            <ul>
                <li>
                    <h1 class="row-title">upcoming events</h1>
                </li>
                <li v-for="el in Listevents" class="text">
                    <div class="date">
                        <p class="day"> {{ el.day }}</p>
                        <p class="month">{{ el.month }}</p>
                    </div>
                    <div class="event">
                        <h2 class="title">{{ el.title }}</h2>
                        <p class="hours">
                            <i class="fa-regular fa-clock"></i>
                            <span>{{ el.time_event }}</span>
                        </p>
                        <p class="place">
                            <i class="fa-solid fa-location-dot"></i>
                            <span>{{ el.place }}</span>
                        </p>
                        <button class="btn">{{ el.btn }}</button>
                    </div>
                </li>
            </ul>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../../style/partials/variables.scss' as *;

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
    background-color: $text-invert;
    max-width: 700px;
}

ul {
    padding: 0;
    margin: 0;
}

li:first-child {
    padding: 20px 200px 20px 40px;
}

li {
    list-style-type: none;
    padding: 30px 200px 30px 40px;
    border-bottom: 1px solid $variant-black;
    background-color: $upcoming;
}

li:first-child:hover {
    transform: none;
}

li:hover {
    background-color: $hover;
    transform: scale(1.1);
}

.text {
    display: flex;
    flex-direction: row;
    align-items: start;
}

.row-title {
    text-transform: capitalize;
    margin: 10px;
}

.date {
    color: $text-invert;
    padding: 10px;
    background-color: $primary;
    text-align: center;
    font-family: $light-font;
    margin-top: 20px;
}

.day {
    font-weight: bold;
    margin: 0;
    font-size: 20px;
    font-family: $light-font;
}

.month {
    font-weight: lighter;
    margin: 0;
}

.event {
    margin: 0 20px;
}

i {
    color: $primary;
    margin-right: 5px;
}

.title {
    text-transform: capitalize;
}

.hours,
.place {
    font-weight: 300;
    font-family: $light-font;
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