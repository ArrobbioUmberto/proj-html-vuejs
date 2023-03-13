<script>
export default {

}
</script>
<template>
    <div class="container" style="position:relative;">
        <div class="row hero">
            <div class="paragraph">
                <h1 class="title">our team</h1>
                <span class="point">.</span>
            </div>
            <p class="description"> Lorem ipsum dolor sit, amet consectetur adipisicing elit. Maxime fugit ut corporis
                commodi
                mollitia magnam molestiae! Facilis est saepe nulla.</p>
            <div class="button-section">
                <button>
                    <span>read more</span>
                    <span class="arrow-button">| &rightarrow;</span>
                </button>
                <button>
                    <span>purchase</span>
                    <span class="arrow-button">| &rightarrow;</span>
                </button>
            </div>
        </div>
        <div class="row_arrow">
            <span class="arrow-left">&LeftArrow;</span> <span class="arrow-right">&RightArrow;</span>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.hero {
    max-width: 600px;
    margin-left: 12.3rem;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: start;
    height: calc(100vh - 100px);
}

.point {
    color: #ff4612;
    font-size: 6rem;
}

.title {
    font-size: 6rem;
    margin: 0;
    text-transform: capitalize;
    font-weight: 600;
}

.paragraph {
    font-size: 3rem;
    display: flex;
}

.description {
    line-height: 30px;
    font-weight: lighter;
}

.row_arrow {
    display: flex;
    justify-content: space-between;
}

.arrow-left,
.arrow-right {
    font-size: 2.3rem;
}

.arrow-left {
    position: absolute;
    top: 50%;
    left: 2rem;
    transform: translate(-50%);
}

.arrow-right {
    position: absolute;
    top: 50%;
    right: 0;
    transform: translate(-50%);
}

.arrow-button {
    padding: 0 10px;
    font-size: 24px;
}

button {
    text-transform: uppercase;
    font-size: 12px;
    padding: 10px 30px;
    margin-right: 15px;
    background-color: white;
    border: none;
}

button:hover {
    color: white;
    background-color: #ff4612;
}
</style>