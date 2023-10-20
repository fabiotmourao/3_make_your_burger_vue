<template>
    <div class="main-banner">
        <h1>Make Your Burger</h1>
    </div>
</template>

<script>
export default {
    name: 'Banner',
}
</script>

<style scoped>
    .main-banner {
        background-image: url('/public/img/burger.jpg');
        background-position: 0 -21.8rem;
        background-size: cover;
        height: 52.7rem;
        display: flex;
        align-items: center;
        justify-content: flex-start;
    }

    .main-banner h1 {
        color: #FCBA03;
        text-align: center;
        font-size: 60px;
        background-color: #222;
        padding: 1.25rem  2.5rem  1.25rem 9rem; 
    }
</style>