<script setup>
        // 定義 emit 事件，用於通知父组件更新 visibleSection
        let emit = defineEmits(['updateSection']);

        function changeSection(section) {
            emit('updateSection', section);  // 觸發事件，通知父组件更新 visibleSection
        }

       
</script>

<template>
  <div class="list">
    <nav class="item" 
         @click="changeSection('CV')">個人簡歷</nav>
    <nav class="item" 
         @click="changeSection('AboutMe')">關於我</nav>
    <nav class="item" 
         @click="changeSection('Plan')">生涯規劃</nav>
    <nav class="item" 
         @click="changeSection('Share')">事件分享</nav>
    </div>

</template>

<style scoped>
    .list{
        display: flex;
        justify-content: center;
        border-bottom-style:solid ;
        margin-bottom: 15px;
        padding: 10px;


    }

    /* 電腦版 */
    @media (min-width: 1025px) {
        .item {
            width: 180px;
            margin: 10px;
            background-color: rgb(250, 140, 5);
            text-align: center;
            border-radius: 10px;
            font-size: 35px;
            cursor: pointer;
            transition: background-color 1s ease, box-shadow 0.2s ease;
        }

        .item:hover {
            background-color: rgb(17, 13, 238);
            color: white;
        }

        .item:active {
            box-shadow: 5px 5px rgb(171, 170, 169);
            font-weight: bold;
        }
    }

    /* 平板版 */
    @media (min-width: 768px) and (max-width: 1024px) {
        .item {
            width: 120px;
            margin: 8px;
            background-color: rgb(250, 140, 5);
            text-align: center;
            border-radius: 8px;
            font-size: 25px;
        }

        .item:hover {
            background-color: rgb(17, 13, 238);
            color: white;
        }

        .item:active {
            box-shadow: 5px 5px rgb(171, 170, 169);
        }
    }

    /* 手機版 */
    @media (max-width: 767px) {
        .item {
            width: 100px;
            margin: 5px;
            background-color: rgb(250, 140, 5);
            text-align: center;
            border-radius: 5px;
            font-size: 15px;
        }

        .item:hover {
            background-color: rgb(17, 13, 238);
            color: white;
        }

        .item:active {
            box-shadow: 5px 5px rgb(171, 170, 169);
        }
    }
    
</style>