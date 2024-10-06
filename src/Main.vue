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
                
                <div class="profile-section">
                    <div>
                        <div class="subtitle">基本資料</div>
                        姓名：張兆丞<br/>
                        性別：男<br/>
                        年齡：27<br/>
                        居住地：新北市蘆洲區<br/>
                    </div>
                    <img src="./asset/head.jpg" alt="头像" />
                </div><br/>

              
                <div class="education-section">
                    <div>
                        <div class="subtitle">學歷</div>
                        <table>
                            <tbody>
                                <tr>
                                    <td>碩士</td>
                                    <td>國立台灣大學生物化學暨分子生物學所</td>
                                </tr>
                                <tr>
                                    <td>學士</td>
                                    <td>國立嘉義大學生化科技學系</td>
                                </tr>
                            </tbody>
                        </table><br/>

                    </div>
                    <img src="./asset/diploma.jpg" alt="畢業證書" />
            </div>
            <div class="subtitle" style="padding-top: 5px;">職業</div>
                        <div>國立陽明交通大學基因體科學研究所專任研究助理</div><br/>
                        <div class="subtitle">工作內容</div>
                        <div>細胞實驗、動物實驗以及資料分析</div><br/>

            <div class="subtitle">申請Bootcamp的契機</div>
            <div>2024年6月份接手以R語言做生物性資料分析，過程中對於寫程式產生興趣，進而開始閱覽彭彭老師的頻道，越做越有信心，也越來越有興趣，在工作上也有利用python寫解讀JSON格式的程式，將JSON資料進行重點抓取並轉移成csv檔。</div><br/>
            
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

        <div class="title">個人簡介和申請動機</div>

        <p class="descript">
            我叫張兆丞，居住於新北蘆洲，今年26歲，畢業於國立台灣大學生物化學暨分子生物學研究所，從事研究助理的工作。主要的職務為操作細胞與動物實驗，隨著科技的進步，生技業也大量的研究引進模型推演以及數據分析，我剛好接觸到生物資訊相關的專案，起初，只會複製貼上程式碼並執行，到後面開始對程式碼的內容產生興趣，因緣際會請教同學時，對方推薦彭彭的課程頻道，從此燃起學習程式語言的熱情。學習一段時間以後，經由老師過往的直播平台發現到工程師轉職計畫，瞬間勾起我的興趣，經過一段時間的思考後，決定參加申請(當時是今年六月)，隨著幾個月的學習，我發現對於寫程式的熱情不增反減，加上看到開訓的時間，完全可以跟我的工作對上(工作合約至年底)，因此，決定在年底後離職並且全職進行轉職計畫。
        </p>
            

        <div class="title">曾經做過哪些軟體工程技術相關的學習？若有作品請分享給我們</div>
        <p class="descript">
            主要觀看彭彭老師於Youtube上傳的程式教學，先從熱門語言python開始學起，之後學習後端框架-Flask，同時，基本介面的渲染也是非常重要， HTML以及CSS成為前端網頁呈現的必備條件，為了讓畫面與使用者更有互動性，學習了前端語言JavaScript以及前端框架-Vue.js，為了解決在開發階段遇到的問題也嘗試去官網、工程師相關論壇以及老師推薦的w3school尋找到合適的解法。
            我利用我所學的後端框架-Flask製作輕量型的python計算機，並且利用前端HTML以及CSS進行版面配置，最後利用前端JavasScript fetch後端運算邏輯，最後呈現在網頁上，我是利用pythonanywhere部屬。看似簡單的小工具，在開發階段也是花費我不少時間，但是在製作過程中也讓我學習到不少技巧，先前學習的技術往往在2週即忘光，給予自己設定一個小小專題，然後完成它，不僅可以加深印象，更能帶給自己成就感。<br/>
            Python 計算機：<a href="https://conan.pythonanywhere.com/">https://conan.pythonanywhere.com/</a> <br/>
            Github 程式碼：<a href="https://github.com/Translation-regulator/Calculator.git" >https://github.com/Translation-regulator/Calculator.git</a>

        </p>

    </div>

    <div v-if="props.visibleSection === 'Plan'">
        <div class="title">如果參與這個訓練，會怎麼安排學習時間？</div>
        <p class="descript">
            我將投入全力學習，並且以全職的身分參加訓練營，除了按部就班跟上老師給予的任務，我將更深入探討任務背後的原理。到了第二階段的實務開發以及團隊開發專案，我期望能與學員於實體活動外建立讀書會，一起交流學習，根據過往開設讀書會的學長姊，相信有助於激發大家的潛能，互相砥礪，並且打磨大家的技術。心態上，我會把訓練營當作碩士二年級即將畢業前半年進行研究，結合開訓前自學的歷程以及bootcamp 前四個月的紮實訓練，最後做出自己的專案，如同寫出論文一樣，我把從bootcamp畢業當作碩士畢業一樣艱辛，所以我將付出更多的時間去完成。
        </p>
        
        <div class="title">軟體技術日新月異，如何確定選擇投入的領域是正確有回報的？</div>
        <p class="descript">
            目前我從事的行業為生物科技，雖然與軟體業一樣技術非常的繁多，但是差別在於生科領域不管是開發出藥物或是解開複雜的病理機制都需要非常非常久的時間，並且常常需要面臨失敗以及經費不足的問題，我個人認為回報率非常低，常常研究到後面失去信心。軟體業現階段除了我們平常使用的網頁以及應用程式以外，現在也跨足到許多行業，像是統計分析以及模型推演，近幾年，醫療業也逐漸開發出幫助判斷的軟體，以及搭配新開發的醫療硬體設備。我目前的工作有一部份也是接受合作實驗室分析出的模型，但是那都是推演，實際在動物的作用情形以及人體實驗也是需要大量時間與金錢去投入。若我加入訓練營，我將朝軟體開發的後端領域進行專精，我認為一個網頁能夠運作的順利，後台的設計非常的重要，不只要運行起來沒問題，運作還不能拖泥帶水，導致使用者體驗非常差。我相信我抱持著的使用者的角度去設計一定可以達到一定的水準，而最大的回報就是薪資，一定也比研究助理來的好。
        </p>
    </div>

    <div v-if="props.visibleSection === 'Share'">
        <div class="title">請描述一件產生明顯負面情緒的經歷，如何處理該情緒？</div>
        <p class="descript">
            我在大四準備考碩士班的過程，對於自己的期望太高，每天壓力極大，真正到了考試的前一晚，焦慮到完全睡不著，當時透過家人的開導以及外出散心，慢慢的將情緒放鬆。有時候第三方的看法能夠跳脫主觀意識，進而讓我面對事情能夠去處理。
        </p>
        
        <div class="title">關於這份申請網頁，分享一個開發時的技術心得</div>
        
            <p class="descript">
                首先，HTML以及CSS的技能是必備的，巢狀的網頁結構以及排版，起初覺得非常簡單，很快即可完成作品上線，直到開發時才發現設計上需要有一定的邏輯。如果巢狀結構沒有精確地使用，即使HTML容錯能力高，未來加入CSS或是JavaScript進行更深層開發容易使程式碼出現問題，除錯的困難度也會大大提升。我使用Vue.js作為前端框架，結合課程中所學，製作響應式網站，並且將網頁區塊進行分類，讓我在除錯以及維護上帶來非常大的便利性，此外，我利用CSS的Media Queries製作適合手機閱讀的版面，歡迎彭彭老師掃描下方QR code參考。最後也是最重要的技術為利用Github Pages將網頁上線，我結合VS code操作介面，順便也了解Git相關的指令，讓我在開發過程中增加許多便利性。<br/>
                Github 程式碼：<a href="https://github.com/Translation-regulator/6th_bootcamp_vue.git">https://github.com/Translation-regulator/6th_bootcamp_vue.git</a>
            </p>
            
            <div class="QRcode"><a href="https://translation-regulator.github.io/6th_bootcamp/"><img src="./asset/Bootcamp.png"></a></div>
   
        <div class="title">如何看待自身工作和整個社會群體的連結關係？</div>
        <p class="descript">
            工作上我比較喜歡不受到限制去發展，像是平常在做研究需要腦力激盪以及豐富的想像力，但是往往被上層給回絕，認為超出傳統的思維就是錯的，為了不想要引發更多的爭執，往往選擇妥協。我認為在群體的工作環境上每個人都是很重要的「螺絲釘」，唯有緊密相扣才能穩健的發展，然而，操控這些螺絲的的工人，也就是主管也是非常重要，將適當的人放在適當的崗位，就要看上位者的智慧。我在群體裏面往往扮演溝通的橋樑，對於我的工作有幫助也有傷害，能幫助我有效與同事交流，交換比次的心得以及技術，但也常常變得多管閒事，因此，近幾年在這方面慢慢取得平衡，既不與團體脫鉤，也不會單方面一頭熱的栽進去。
        </p>
        
        <div class="title">其他想要對我們說的事情？</div>
        <p class="descript">
            感謝彭彭老師開設WeHelp-軟體工程師專業社群扶持計畫，讓大家有機會從無到有一步一腳印完成自己的理想與夢想，也感謝老師開設的Youtube頻道，淺顯易懂的內容使我在一開始就愛上程式設計，並且也讓我找到額外的興趣，看著一行一行的程式碼運作起來，自己的成就感也油然而生，從一開始僅為了訓練腦袋邏輯到自己製作小程式應用在工作上，現階段對軟體工程師有一定的嚮往，也希望能夠成功轉職。因此，我給我自己的期許也給老師的承諾，如果有幸加入第六屆bootcamp的訓練營，我將義無反顧並且全心全力的完成每次任務，即使有空檔的時間，也將不斷的學習，套用老師頻道的一句話「穩定承諾，終身學習」。
        </p>
        
    </div>

    </main>
</template>

<style scoped>
    .content {

        flex-wrap: wrap;
        width: 70%;
    }

    table, th, td {
        border: 4px solid black;
        border-collapse: collapse;
    }

    .InnerContent {
        padding-top: 3%;
    }

    .title {
        font-weight: bold;
        font-size: 30px;
    }

    .descript {
        font-size: 26px;
        font-family: 'Times New Roman', serif, 'DFKai-sb', sans-serif;
        line-height: 45px;
        text-align: justify;
    }

    .subtitle {
        font-size: 30px;
        font-weight: bold;
        text-decoration: underline;
        margin-bottom: 5px;
    }

    .profile-section, .education-section {
        display: flex;
        justify-content: space-between;
        align-items: flex-start;
    }

    .profile-section img, .education-section img {
        width: 150px;
    }

    .education-section img {
        width: 400px;
    }

    /* 電腦版 */
    @media only screen and (min-width: 1024px) {
        .InnerContent {
            width: 60%;
        }
    }

    /* 平板版 */
    @media only screen and (min-width: 768px) and (max-width: 1024px) {
        .InnerContent {
            width: 80%;
        }

        .title, .subtitle {
            font-size: 24px;
        }

        .descript {
            font-size: 22px;
            line-height: 36px;
        }
    }

    /* 手機版 */
    @media only screen and (max-width: 767px) {
        .InnerContent {
            width: 95%;
            padding: 5%;
        }

        .title {
            font-size: 20px;
        }

        .subtitle {
            font-size: 18px;
        }

        .descript {
            font-size: 18px;
            line-height: 30px;
        }

        /* 將大頭照移至基本资料上方 */
        .profile-section {
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .profile-section img {
            order: -1; /* 將大頭照放在文字上方 */
            margin-bottom: 20px;
        }

        /* 將畢業證書移至學歷下方 */
        .education-section {
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .education-section img {
            margin-top: 20px;
            width: 300px;
        }

        .QRcode{
            display: none;
        }
    }
</style>

