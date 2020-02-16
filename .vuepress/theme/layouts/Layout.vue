<template>
    <div>
        <Nav />
        <div class="body-container">
            <div class="body-content">
                <Content />
            </div>
        </div>
    </div>
</template>

<style lang="scss">
@import url('https://fonts.googleapis.com/css?family=Roboto+Mono:400,700&display=swap');

@keyframes fadeIn {
    from {
        opacity: 0;
        transform: scale(0.98)
    }

    to {
        opacity: 1;
        transform: scale(1)
    }
}

@keyframes rainbow { 
    0%{background-position:0% 82%}
    50%{background-position:100% 19%}
    100%{background-position:0% 82%}
}

html {
    animation: fadeIn 0.4s ease-out;
}

body {
    font-family: 'Roboto Mono', sans-serif;
}

blockquote {
    background: rgba(yellow, 0.2);
    border-left: 5px solid #000;
    p, h1, h2, h3, h4, h5 {
        padding: 10px 20px;
        margin: 0;
    }
}

</style>

<style lang="scss" scoped>

.body-container {
    box-sizing: border-box;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

.body-content {
    position: relative;
    max-width: 950px;
    padding: 0 50px;
    min-height: 95vh;
    background: rgba(white, 0.5);
}
</style>

<script>
    import Nav from "@theme/components/Nav"
    import 'normalize.css'

    export default {
        components: {
            Nav
        }
    }
</script>