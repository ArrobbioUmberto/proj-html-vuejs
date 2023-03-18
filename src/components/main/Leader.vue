<script>
export default {
    data() {
        return {
            Percentage: [
                {
                    title_perc: 'mentorship',
                    number_perc: '78%'
                },
                {
                    title_perc: 'education',
                    number_perc: '95%'
                },
                {
                    title_perc: 'learning',
                    number_perc: '65%'
                },
                {
                    title_perc: 'motivation',
                    number_perc: '83%'
                }
            ]
        }
    }
}
</script>
<template>
    <div class="container">
        <div class="row">
            <div class="col section-left">
                <div class="leader">
                    <h1 class="title">creative leader</h1>
                    <span class="point">.</span>
                </div>
                <span class="line"></span>
                <p class="text">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Enim numquam laboriosam optio!
                    Vitae accusamus deleniti, fugiat temporibus laudantium nobis consectetur dolores? Ab, possimus nostrum.
                    Id quam optio totam. Sequi odit obcaecati, illo possimus autem tenetur rem?
                    Delectus iure error consequuntur sapiente odio magnam eos. Quod enim obcaecati possimus.</p>
                <button class="btn">read more</button>
            </div>
            <div class="col">
                <div v-for="el in Percentage">
                    <div class="percentuale">
                        <h2 class="title_perc">{{ el.title_perc }}</h2>
                        <span class="number_perc">{{ el.number_perc }}</span>
                    </div>
                    <span class="loader" :style="{ width: el.number_perc }"></span>
                </div>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../../style/partials/variables.scss' as *;

.row {
    display: flex;
    flex-direction: row;
    max-width: 1380px;
    margin: 0 auto;
    gap: 7.5rem;
}

.col {
    display: flex;
    flex-direction: column;
    flex-basis: 50%;
}

.leader {
    display: flex;
    flex-direction: row;
    align-items: baseline;
}

.title {
    text-transform: capitalize;
    font-size: 2.5rem;
    margin: 0;
}

.point {
    color: $primary;
    font-size: 2.5rem;
}

.line {
    border-bottom: 2px solid $primary;
    display: inline-block;
    width: 9%;
    padding: 5px;
}

.text {
    font-size: 1.2rem;
    font-weight: 300;
    font-family: $light-font;
    line-height: 1.75rem;
}

.btn {
    border: none;
    background-color: transparent;
    text-transform: uppercase;
    font-weight: 600;
    font-size: 0.8rem;
    text-align: start;
}

.percentuale {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    border-bottom: 1px solid $variant-black;
    margin-bottom: -1rem;
}

.title_perc {
    text-transform: capitalize;
    font-size: 1.2rem;
    margin: 0;
    padding: 1.4rem 0;
    font-weight: bold;
}

.number_perc {
    font-weight: bold;
    font-size: 1.2rem;
}

.loader {
    display: inline-block;
    background-color: $primary;
    height: 5px;
}
</style>