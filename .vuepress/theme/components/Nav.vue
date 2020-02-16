<template>
    <div class="nav-container">
        <h1 class="title">OPEN @ OLIN</h1>
    </div>
</template>

<style scoped lang="scss">
.title {
    font-size: 3em;
    position: relative;
    width: 100%;
    max-width: 950px;
    animation: rainbow 18s ease infinite;
    background: linear-gradient(124deg, #ff2400, #e81d1d, #e8b71d, #e3e81d, #1de840, #1ddde8, #2b1de8, #dd00f3, #dd00f3);
    background-size: 1800% 1800%;
    color: transparent;
    background-clip: text;
    margin: 20px auto;
}

.nav-container {
    box-sizing: border-box;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;  
    background: rgba(white, 0.3);
    padding: 0 50px;
}
</style>

<script>
export default {
    name: 'Nav',
    data() {
        return {}
    }
}
</script>