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