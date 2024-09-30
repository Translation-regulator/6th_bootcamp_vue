<script setup>
        // 接收来自父组件傳遞的 visibleSection prop
        let props = defineProps({
        visibleSection: String
        });
</script>

<template>
    <main class="InnerContent">
    <div v-if="props.visibleSection === 'CV'">
        
        <div class="descript">
            <div style="display: flex;">
                <div style="padding-right: 65%;">
                    <div class="subtitle">基本資料</div>
                        姓名：張兆丞<br/>
                        性別：男<br/>
                        年齡：27<br/>
                        居住地：新北市蘆洲區<br/>
                </div>
                <div>
                    <img src="./asset/head.jpg" style="width: 150px">
                </div>
            </div>
            <div class="subtitle">學歷</div>
            <table>
                <tr>
                    <td>碩士</td>
                    <td>國立台灣大學生物化學暨分子生物學所</td>
                </tr>
                <tr>
                    <td>學士</td>
                    <td>國立嘉義大學生化科技學系</td>
                </tr>
            </table>
            <div class="subtitle" style="padding-top: 5px;">職業</div>
            國立陽明交通大學基因體科學研究所
            專任研究助理
            <br/>

            <div class="subtitle">工作內容</div>
            細胞實驗、動物實驗以及資料分析<br/>

            <div class="subtitle">申請Bootcamp的契機</div>
            2024年6月份接手以R語言做生物性資料分析，過程中對於寫程式產生興趣，進而開始閱覽彭彭老師的頻道，越做越有信心，也越來越有興趣，在工作上也有利用python寫解讀JSON格式的程式，將JSON資料進行重點抓取並轉移成csv檔。<br/>
            
            <div class="subtitle">參加訓練營的規劃</div>

            <div style="font-weight: bold;">短期(訓練前~訓練前期)</div>
            利用下班以及假日的時間學習程式開發，直到年底合約到期將提離職並全職參與訓練營，一天至少投入8~10小時進行程式學習以及開發。<br>

            <div style="font-weight: bold">中期(第二階段~結訓)</div>
            努力完成訓練營交辦事項，從中再延伸出更多的學習目標，同時，最終將精進於後端開發，並且獨力完成後端專案。<br>

            <div style="font-weight: bold">後期(以軟體工程師身分就業)</div>
            辛苦6個月的密集訓練，從訓練營畢業後，初份工作將以後端工程師為主要目標，並且從做中學，期望5年內能成為全端工程師(自我期許)。<br>

            



        </div>
    </div>
    <div v-if="props.visibleSection === 'AboutMe'">

        <div class="title">個人簡介</div>

        <p class="descript">我叫張兆丞，居住於新北蘆洲，今年26歲，畢業於國立台灣大學生物化學暨分子生物學研究所，從事研究助理的工作。主要的職務為操作細胞與動物實驗，隨著科技的進步，生技業也大量的研究引進模型推演以及數據分析，我剛好接觸到生物資訊相關的專案，起初，只會複製貼上程式碼並執行，到後面開始對於程式碼的內容產生興趣，因緣際會請教同學時，對方推薦彭彭的課程頻道，從此燃起對於學習程式語言的熱情。
        </p>
            

        <div class="title">為了成為軟體工程師，做過什麼努力？若有具體作品請分享給我們</div>
        <p class="descript">主要觀看彭彭老師於Youtube上傳的程式教學，先從熱門語言python開始學起，之後學習後端框架-Flask，同時，基本介面的渲染也是非常重要， HTML以及CSS成為前端網頁呈現的必備條件，為了讓畫面與使用者更有互動性，學習了前端語言JavaScript以及前端框架-Vue.js，為了解決在開發階段遇到的問題也嘗試去官網、工程師相關論壇以及老師推薦的w3school尋找到合適的解法。</p>

    </div>

    <div v-if="props.visibleSection === 'Plan'">
        <div class="title">如果參與這個訓練，會怎麼安排學習時間？</div>
        <p class="descript">我將投入全力學習，並且以全職的身分參加訓練營，除了按部就班跟上老師給予的任務，我將更深入探討任務背後的原理。到了第二階段的實務開發以及團隊開發專案，我期望能與學員於實體活動外建立讀書會，一起交流學習，根據過往開設讀書會的學長姊，相信有助於激發大家的潛能，互相砥礪，並且打磨大家的技術。
        </p>
        
        <div class="title">是否有想要加入的公司？為什麼想加入該公司？</div>
        <p class="descript">有鑑於長期對於股市有小小的研究，因此想加入財報狗-股市分析的公司或是玉山銀行、元大投信等金融機構。學生時期對於使用軟體分析股票感到相當好奇，也曾想過自己能創造出超越市面上的網站，經過多年以後，終於可以完成我的願望!參考了WeHelp的Demo Day，看到許多學長姐分享設計的看盤軟體以及心路歷程，萌生我加入訓練營的挑戰。
        </p>
    </div>

    <div v-if="props.visibleSection === 'Share'">
        <div class="title">請描述一件產生明顯負面情緒的經歷，如何處理該情緒？</div>
        <p class="descript">我在大四準備考碩士班的過程，對於自己的期望太高，每天壓力極大，真正到了考試的前一晚，焦慮到完全睡不著，當時透過家人的開導以及外出散心，慢慢的將情緒放鬆。有時候第三方的看法能夠跳脫主觀意識，進而讓我面對事情能夠去處理。</p>
        
        <div class="title">關於這份申請網頁，分享一個開發時的技術心得</div>
        <p class="descript">首先，HTML以及CSS的技能是必備的，巢狀的網頁結構以及排版，起初覺得非常簡單，很快即可完成作品上線，直到開發時才發現設計上需要有一定的邏輯。如果巢狀結構沒有精確地使用，即使HTML容錯能力高，未來加入CSS或是JavaScrip進行更深層開發容易使程式碼出現問題，除錯的困難度也會大大提升。最後也是最重要的技術為利用Github Pages將網頁上線，我結合VS code操作介面，順便也了解Git相關的指令，讓我在開發過程中增加許多便利性。
        </p>
        
        <div class="title">請用簡短兩三句話，描述對你而言，最重要的一項人際交往原則</div>
        <p class="descript">我的個性屬於開朗活潑，並且屬於容易混入群體的個體，因此在社交上並無太大的阻礙，期望加入訓練營能夠與大家融洽的相處。 </p>
        
        <div class="title">其他想要對我們說的事情？</div>
        <p class="descript">感謝彭彭老師開設WeHelp-軟體工程師專業社群扶持計畫，讓大家有機會從無到有一步一腳印完成自己的理想與夢想，也感謝老師開設的Youtube頻道，淺顯易懂的內容使我在一開始就愛上程式設計，並且也讓我找到額外的興趣，看著一行一行的程式碼運作起來，自己的成就感也油然而生。因此，我給我自己的期許也給老師的承諾，如果有幸加入第六屆bootcamp的訓練營，我將義無反顧並且全心全力的完成每次任務，即使有空檔的時間，也將不斷的學習，套用老師頻道的一句話「穩定承諾，終身學習」。</p>
        
    </div>

    </main>
</template>

<style scoped>
    .content{
        display: flex;
        flex-wrap: wrap;

    }

    table, th, td {
        border: 2px solid black;
        border-collapse: collapse;
    }

    .InnerContent{
        flex:none; width: 60%;
        padding: 3%;
        
    }
    .title{
        font-weight: bold;
        font-size: 28px;
    }

    .descript{
        font-size: 20px;
        font-family: 'Times New Roman', serif,'DFKai-sb', sans-serif;
        line-height: 40px;
        text-align: justify; /** 使文字左右對齊 **/
    }
    .subtitle{
        font-size: 24px;
        font-weight: bold;
        text-decoration: underline;
        margin-bottom: 5px;
    }
</style>