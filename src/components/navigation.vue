<template>
    <div class="navigation">
        <nav class="menu">
            <h1>COLORS˚</h1>
            <span>ПРОДУКТЫ</span>
            <span>ЦВЕТА</span>
            <span>ВДОХНОВЕНИЕ</span>
            <span>СОВЕТЫ</span>
            <span>НАЙТИ МАГАЗИН</span>
        </nav>
        <div class="tel">
            <a href="tel:+7(495)221-77-69">+7 (495) 221-77-69</a>
            <p>Заказать звонок</p>
        </div>
        <div class="search">
            <img src="../assets/images/search.png" alt="">
            <img src="../assets/images/profile.png" alt="">
            <img src="../assets/images/heart.png" alt="">
            <button class="cart-btn">{{}}</button>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'navigation'
    }
</script>

<style scoped>
    .navigation {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        align-items: center;
        height: 104px;
        left: 0px;
        top: 0px;
        background: #FFFFFF;
    }   
    .menu{
        display: flex;
        flex-direction: row;
        align-items: center;
    }
    .menu span {
        font-family: Inter;
        font-style: normal;
        font-weight: normal;
        font-size: 14px;
        margin-left: 24px;
    }
    .menu span:hover {
        cursor: pointer;
        border-bottom: 4px solid #7BB899;
        transition: ease-in 0.25s;
        transform: scale(1.1);
    }
    .search {
        display: flex;
        font-display: row;
        margin-right: 14px;
    }
    .search img {
        margin-right: 26px;
    }
    h1 {
        margin-left: 64px;
    }
    a {
        text-decoration: none;
        color: #000;
    }
    p {
        margin: 0;
        font-size: 0.75rem;
        color: grey;
    }
    .cart-btn {
        border: none;
        background-color: #7BB899;
        height: 24px;
        width: 24px;
        border-radius: 50%;
    }
</style>