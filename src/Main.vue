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
                        年齡：26<br/>
                        居住地：新北市蘆洲區<br/>
                    </div>
                    <img src="./asset/head.jpg" alt="大頭照" />
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

        </div>
    </div>
    <div v-if="props.visibleSection === 'AboutMe'">

        <div class="title">個人簡介和申請動機</div>

        <p class="descript">
            我叫張兆丞，今年26歲，居住於新北市蘆洲，畢業於國立台灣大學生物化學暨分子生物學研究所，目前擔任專任研究助理，我的工作主要操作細胞和動物實驗。隨著科技的進步，生技產業越來越多地運用模型推演和數據分析，自2024年6月起，我開始使用R語言進行生物數據分析，並在工作中運用Python撰寫程式來解讀JSON資料，將其轉換為CSV文件。<br/>
            起初，我只是在工作中執行現有的程式碼，但隨著時間推移，我對程式設計逐漸產生了濃厚興趣。在一次與同學討論時，他向我推薦了彭彭的課程頻道，從此激發了我學習程式語言的熱情。隨著學習的深入，我透過老師的直播課程發現了工程師轉職計畫，這立即引起了我的強烈興趣。經過一段時間的考慮，我在今年7月決定申請，並且期望能夠參加第六屆bootcamp。<br/>
            幾個月的學習讓我更加堅定了轉職的決心。我發現自己對程式設計的熱情隨著時間慢慢增加，因此我計劃在年底辭去現有工作，全力以赴投入這次轉職旅程。
        </p>
            

        <div class="title">曾經做過哪些軟體工程技術相關的學習？若有作品請分享給我們</div>
        <p class="descript">
            主要是觀看彭彭老師在YouTube上傳的程式教學，從熱門語言Python開始學習，接著學習後端框架Flask。同時，基本介面的渲染也非常重要，因此學習了HTML和CSS，這是前端網頁呈現的必要條件。為了讓畫面更具互動性，我學習了前端語言JavaScript以及前端框架Vue.js。在開發過程中，為了解決遇到的問題，我會查閱官方文件、工程師論壇，以及老師推薦的w3school，尋找合適的解決辦法。<br/>
            我利用學到的Flask框架製作了一個輕量級的Python計算機，並使用HTML和CSS進行版面配置，最後用JavaScript的fetch方法來調用後端的運算邏輯，並將結果呈現在網頁上。我使用PythonAnywhere進行部署。雖然這個小工具看似簡單，但在開發過程中花費了不少時間，讓我學到了許多技巧。與過去學習不同的是，之前學的技術常常兩週後就忘記了，但這次給自己設計了一個小專案並完成它，不僅加深了記憶，也帶給我成就感。我將計算機的網址傳給親朋好友，請大家以使用者角度給予我建議，因此，當我收到建議後，我會一直進行修改。<br/>
            <a href="https://conan.pythonanywhere.com/">Python 計算機</a><br/>
            <a href="https://github.com/Translation-regulator/Calculator.git" >Github 程式碼</a>
        </p>
        <span style="text-align:left;">

        </span>

    </div>

    <div v-if="props.visibleSection === 'Plan'">
        <div class="title">如果參與這個訓練，會怎麼安排學習時間？</div>
        <p class="descript">
            我將以全職身分全力參加訓練營，每日分配至少8小時進行程式開發以及相關背景知識的閱覽，除了按時完成課程作業外，我也會深入理解每個任務背後的原理。進入實務開發和團隊專案階段後，我希望能與其他學員組織讀書會，彼此交流學習。根據學長姊的經驗，讀書會能有效提升技術能力並激發潛能。<br/>
            心態上，我將訓練營視為碩士論文衝刺的最後階段，結合自學和訓練營四個月的密集訓練，期望在結業時能完成自己的專案，就像完成論文一般。對我來說，訓練營的挑戰與碩士畢業一樣嚴苛，因此我將全力以赴，投入更多時間與精力，力求成功。<br/>
            <span style="font-weight: bold;">短期目標(申請後~進入訓練營前)</span><br/>
            在申請後到 2025/1/6 之前，我會研究 Python 的 FastAPI 框架，為進入訓練營做準備。同時，會加強 JavaScript 的語法，再完成一個小型專案。如果時間允許，也會專研資料結構與演算法，因為這些是未來學習中重要的基石。<br/>
            <span style="font-weight: bold;">中期目標(前兩階段的訓練)</span><br/>
            我將專注於精進程式技術，按時完成每次任務，並養成閱覽官方文件的習慣，製作個人的學習筆記以備後續開發使用。我會將重心放在後端開發，期望能夠在訓練營結束時，具備後端工程師的能力。<br/>
            <span style="font-weight: bold;">長期目標(第三階段~完成就業)</span><br>
            經過前兩階段的學習，我相信自己能獨立完成軟體開發，專案將以後端作品為主。順利就業後，我期許自己在 5 年內成為全端工程師，不斷提升專業能力。
        </p>
        
        <div class="title">軟體技術日新月異，如何確定選擇投入的領域是正確有回報的？</div>
        <p class="descript">
            我目前從事的行業是生物科技。雖然這個領域的技術非常繁複，但不同於軟體業，生科領域不管是藥物開發還是解開複雜的病理機制，都需要很長的時間，並且常常面臨失敗和資金不足的挑戰，回報率相對較低，這讓我在長期研究後容易失去信心。相比之下，軟體行業的發展速度更快，不僅應用於我們日常使用的網站和應用程式，還參與到統計分析、模型推演，甚至醫療行業，開發出輔助判斷的軟體與新型醫療硬體設備。我的工作中也接觸到合作實驗室的數據模型分析，但這些模型仍需在動物實驗和臨床試驗中耗費大量時間和金錢去驗證。<br/>
            如果我加入訓練營，我會專注於軟體開發的後端領域。我認為一個網站能夠順利運作，後台的設計至關重要，不僅要確保運行無誤，還要保證性能高效，避免影響使用者體驗。我相信，從使用者的角度出發來設計後端架構，能夠達到較高的水準。最直接的回報就是薪資，我堅信轉職成為軟體工程師的薪酬和職業發展機會都會遠勝於我目前的研究助理工作。
        </p>
    </div>

    <div v-if="props.visibleSection === 'Share'">
        <div class="title">請描述一件產生明顯負面情緒的經歷，如何處理該情緒？</div>
        <p class="descript">
            我在大四準備考碩士班的過程，對於自己的期望太高，每天壓力極大，真正到了考試的前一晚，焦慮到完全睡不著，當時透過家人的開導以及外出散心，慢慢的將情緒放鬆。有時候第三方的看法能夠跳脫主觀意識，進而讓我面對事情能夠冷靜的去處理，並且做出最有利的判斷。
        </p>
        
        <div class="title">關於這份申請網頁，分享一個開發時的技術心得</div>
        
         <p class="descript">
            首先，HTML和CSS是網頁開發中必備的技能。起初，我認為巢狀結構和排版相對簡單，能很快完成上線。然而，在實際開發過程中我發現，設計結構需要具備一定的邏輯性。如果巢狀結構沒有正確使用，即使HTML的容錯能力較高，未來在加入CSS或JavaScript進行更深入的開發時，容易導致問題，並增加除錯的難度。為了提高開發效率，我使用Vue.js作為前端框架製作響應式網站，根據課程所學，將網站區塊進行合理分類，這不僅讓除錯更容易，也大大提升了後續的維護性。<br/>
            此外，我利用CSS的Media Queries確保網頁在手機端也能有良好的瀏覽體驗。最後，為了讓網頁順利上線，我使用了GitHub Pages，並透過VS Code的操作介面進行Git相關指令的操作，這大大提升了開發的便利性。歡迎彭彭老師掃描下方QR code，查看手機版本。
            <br/>
            <a href="https://github.com/Translation-regulator/6th_bootcamp_vue.git">Github 程式碼</a>
         </p>
            
            <div class="QRcode"><a href="https://translation-regulator.github.io/6th_bootcamp/"><img src="./asset/Bootcamp.png"></a></div>
   
        <div class="title">如何看待自身工作和整個社會群體的連結關係？</div>
        <p class="descript">
            在工作中，我傾向於追求較大的自由度，尤其是在研究過程中，我喜歡發揮豐富的想像力進行創新思考。然而，這樣的創意常常遭到上層的否決，因為在某些傳統思維模式下，超出常規的想法容易被視為錯誤。為了避免衝突，我時常選擇妥協。<br/>
            我認為，在一個群體的工作環境中，每個人都是一個關鍵的「螺絲釘」，只有彼此緊密協作，才能確保整個機制平穩運行。而作為管理者，他們就像操控這些螺絲的技工，決定了如何把合適的人放在合適的崗位上。這需要很高的智慧與洞察力。在這樣的架構中，我通常專注於完成自己的任務，不會過多摻雜額外的個人想法，這既有助於團隊的和諧，也避免了不必要的衝突。<br/>
            作為團體中的一員，我的角色往往是充當溝通的橋樑，這對我的工作既有益處，也有挑戰。它幫助我更有效地與同事交流，分享彼此的經驗和技術，但有時也容易讓我陷入多管閒事的困境。因此，近年來，我學會了在這方面找到一個平衡點，既不與團體脫節，也不會過度鑽牛角尖，這樣的平衡讓我在群體中發揮了更大的作用，也提高了工作的滿意度。
        </p>
        
        <div class="title">其他想要對我們說的事情？</div>
        <p class="descript">
            感謝彭彭老師開設 WeHelp-軟體工程師專業社群扶持計畫，讓我們有機會從零開始，一步步實現自己的理想與夢想。也感謝老師的 YouTube 頻道，淺顯易懂的教學內容讓我一開始就愛上了程式設計，並激發了我的興趣。從僅僅為了訓練邏輯思維到能夠製作小程式應用於工作上，程式設計帶給我無比的成就感。<br/>
            現在，我對成為軟體工程師充滿嚮往，也希望能藉此成功轉職。若有幸加入第六屆 Bootcamp 訓練營，我承諾將全力以赴，完成每一項任務。即使在空檔時間，也會不斷學習，精進自己。正如老師頻道中的一句話：「穩定承諾，終身學習」，我將銘記在心。
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

    .profile-section img {
        width: 10vw;
    }

    .education-section img {
        width: 23vw;
    }

    /* 電腦版 */
    @media only screen and (min-width: 1024px) {
        .InnerContent {
            width: 70%;
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

            .profile-section img {
            width: 15vw;
        }

        .education-section img {
            width: 25vw;
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
            width: 30vw;
        }

        /* 將畢業證書移至學歷下方 */
        .education-section {
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .education-section img {
            margin-top: 20px;
            width: 80vw;
        }

        .QRcode{
            display: none;
        }
    }
</style>

