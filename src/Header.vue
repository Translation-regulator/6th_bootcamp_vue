<script setup>

</script>

<template>
    <header>
        <h1 class="desktop">第六屆WeHelp軟體工程師轉職計畫</h1>
        <h1 class="mobile">WeHelp工程師轉職計畫</h1>
    </header>
</template>

<style scoped>
    h1{
        text-align: center;
        font-size: 50px;
        text-shadow: 2px 2px 5px rgb(250, 140, 5);
    }

    h1.desktop {
        display: block;
    }

    h1.mobile {
        display: none;
    }

    /* 電腦版 */
    @media (min-width: 1025px) {
        h1.desktop {
            display: block;
        }
        
        h1.mobile {
            display: none;
        }
    }

    /* 平板版 */
    @media (min-width: 768px) and (max-width: 1024px) {
        h1.desktop {
            display: none;
        }

        h1.mobile {
            display: block;
            font-size: 40px;
        }
    }

    /* 手機版 */
    @media (max-width: 767px) {
        h1.desktop {
            display: none;
        }

        h1.mobile {
            display: block;
            font-size: 30px;
        }
    }
</style>