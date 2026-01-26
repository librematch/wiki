# [GET] /community/news/getNews

[Example request](https://aoe-api.worldsedgelink.com/community/news/getNews?title=age2)

## Request

| parameter | type     | value                  | comments |
| --------- | -------- | ---------------------- | -------- |
| title     | str/enum | age1, age2, age3, age4 |          |

## Response

### AoE2:DE

```
{
  "result": {
    "code": 0,
    "message": "SUCCESS"
  },
  "news": [
    {
      "id": 822,
      "hidden": 0,
      "newscategory": "(01/17) 56 en",
      "newstitle_locstringid": -1,
      "newssubtitle_locstringid": -1,
      "newstext_locstringid": -1,
      "newsimage": "Red Bull Wololo: Legacy Tournament October 21 - 30",
      "newsbody": "To battle! Red Bull Wololo is back, bringing together the best Age of Empires players from around the world for a battle of the ages. Will TheViper defend his title, or will one of the aspiring competitors be crowned the true ruler of Castle Heidelberg? \n\nRed Bull Wololo: Legacy runs from October 21 to October 30. Tune in here to catch all the action: twitch.tv/redbull.",
      "metadata": "NEWS;id=56;lang=en",
      "datevisible": 1666386000,
      "expirytime": 1667196000
    },
    {
      "id": 823,
      "hidden": 0,
      "newscategory": "(02/17) 56 zh",
      "newstitle_locstringid": -1,
      "newssubtitle_locstringid": -1,
      "newstext_locstringid": -1,
      "newsimage": "红牛呜噜噜：旧版锦标赛 10 月 21 日至 30 日",
      "newsbody": "战斗！红牛呜噜噜又回来啦，汇集了来自世界各地的最佳《帝国时代》玩家，展开一场世纪之战。TheViper 会捍卫他的头衔，还是一名有抱负的竞争对手会加冕为海德堡城堡的真正统治者？\n\n\"\"红牛呜噜噜：旧版锦标赛\"\"举行时间为 10 月 21 日到 10 月 30 日。敬请锁定以下网站，观看所有精彩镜头：twitch.tv/redbull。",
      "metadata": "NEWS;id=56;lang=zh",
      "datevisible": 1666386000,
      "expirytime": 1667196000
    },
    {
      "id": 824,
      "hidden": 0,
      "newscategory": "(03/17) 56 tw",
      "newstitle_locstringid": -1,
      "newssubtitle_locstringid": -1,
      "newstext_locstringid": -1,
      "newsimage": "紅牛嗚嚕嚕 (Red Bull Wololo: Legacy) 錦標賽 10 月 21 日至 30 日",
      "newsbody": "戰鬥吧！紅牛嗚嚕嚕又回來了，匯集了 Age of Empires 來自世界各地的頂尖玩家，進行一場時代之戰。TheViper 會捍衛他的寶座，還是其他胸懷大志的競爭對手會加冕成為 Heidelberg 城堡的真正統治者？\n\n紅牛嗚嚕嚕 (Red Bull Wololo: Legacy) 舉行期間為 10 月 21 日到 10 月 30 日。請在以下頻道收看，不要錯過任何精彩片刻：twitch.tv/redbull。",
      "metadata": "NEWS;id=56;lang=tw",
      "datevisible": 1666386000,
      "expirytime": 1667196000
    },
    {
      "id": 825,
      "hidden": 0,
      "newscategory": "(04/17) 56 fr",
      "newstitle_locstringid": -1,
      "newssubtitle_locstringid": -1,
      "newstext_locstringid": -1,
      "newsimage": "Tournoi Red Bull Wololo : Héritage du 21 au 30 octobre",
      "newsbody": "Au combat ! Red Bull Wololo est de retour avec les meilleurs joueurs d’Age of Empires pour une bataille qui restera dans les annales. TheViper conservera-t-il son titre de souverain du château de Heidelberg, ou sera-t-il détrôné par l'un de ses compétiteurs ?\n\nRed Bull Wololo : Héritage se déroule du 21 au 30 octobre. Rendez-vous ici pour suivre toute l’action : twitch.tv/redbull.",
      "metadata": "NEWS;id=56;lang=fr",
      "datevisible": 1666386000,
      "expirytime": 1667196000
    },
    {
      "id": 826,
      "hidden": 0,
      "newscategory": "(05/17) 56 de",
      "newstitle_locstringid": -1,
      "newssubtitle_locstringid": -1,
      "newstext_locstringid": -1,
      "newsimage": "Red Bull Wololo: Legacy-Turnier 21.–30. Oktober",
      "newsbody": "Auf in den Kampf! Red Bull Wololo ist zurück und bringt die besten Age of Empires-Spieler aus der ganzen Welt für einen Kampf durch die Age-Geschichte zusammen. Wird TheViper seinen Titel verteidigen? Oder wird einer der aufstrebenden Konkurrenten zum wahren Herrscher von Schloss Heidelberg gekrönt?\n\nRed Bull Wololo: Legacy findet vom 21. bis 30. Oktober statt. Schalten Sie hier ein, um die ganze Action zu sehen: twitch.tv/redbull.",
      "metadata": "NEWS;id=56;lang=de",
      "datevisible": 1666386000,
      "expirytime": 1667196000
    },
    {
      "id": 827,
      "hidden": 0,
      "newscategory": "(06/17) 56 hi",
      "newstitle_locstringid": -1,
      "newssubtitle_locstringid": -1,
      "newstext_locstringid": -1,
      "newsimage": "रेड बुल वोलोलो: विरासत टूर्नामेंट 21 - 30 अक्टूबर",
      "newsbody": "लड़ाई के लिए! रेड बुल वोलोलो वापस आ गया है, युगों की लड़ाई के लिए दुनिया भर के सर्वश्रेष्ठ एज ऑफ एम्पायर खिलाड़ियों को एक साथ ला रहा है। क्या द वाइपर अपने खिताब की रक्षा करेगा, या आकांक्षी प्रतियोगियों में से एक को कैसल हीडलबर्ग के सच्चे शासक का ताज पहनाया जाएगा?\n\nरेड बुल वोलोलो: विरासत 21 अक्टूबर से 30 अक्टूबर तक चलती है। सभी एक्शन देखने के लिए यहां ट्यून करें: twitch.tv/redbull।",
      "metadata": "NEWS;id=56;lang=hi",
      "datevisible": 1666386000,
      "expirytime": 1667196000
    },
    {
      "id": 828,
      "hidden": 0,
      "newscategory": "(07/17) 56 it",
      "newstitle_locstringid": -1,
      "newssubtitle_locstringid": -1,
      "newstext_locstringid": -1,
      "newsimage": "Torneo Red Bull Wololo: Legacy, 21-30 ottobre",
      "newsbody": "Alla battaglia! Red Bull Wololo è tornato. I migliori giocatori di Age of Empires da tutto il mondo sono chiamati a raccolta per una battaglia epocale. Riuscirà TheViper a difendere il suo titolo o sarà uno degli aspiranti contendenti a essere incoronato sovrano del castello di Heidelberg?\n\nRed Bull Wololo: Legacy si svolgerà dal 21 al 30 ottobre. Sintonizzati qui per seguire tutte le sfide: twitch.tv/redbull.",
      "metadata": "NEWS;id=56;lang=it",
      "datevisible": 1666386000,
      "expirytime": 1667196000
    },
    {
      "id": 829,
      "hidden": 0,
      "newscategory": "(08/17) 56 jp",
      "newstitle_locstringid": -1,
      "newssubtitle_locstringid": -1,
      "newstext_locstringid": -1,
      "newsimage": "レッドブル ウォロロ: レガシー トーナメント 10 月 21 日 - 30 日",
      "newsbody": "いざ戦場へ! レッドブル ウォロロが帰ってきました。世界中から集った最高の Age of Empires プレイヤーが、時代を超えた戦いを繰り広げます。はたして TheViper はタイトルを防衛できるでしょうか? それとも闘志を燃やすライバルの誰かが新たな王者として戴冠するのでしょうか?\n\nレッドブル ウォロロ: レガシーは、10 月 21 日から 10 月 30 日にかけて開催されます。熱戦の様子は以下のチャンネルで余すところなくご覧いただけます: twitch.tv/redbull",
      "metadata": "NEWS;id=56;lang=jp",
      "datevisible": 1666386000,
      "expirytime": 1667196000
    },
    {
      "id": 830,
      "hidden": 0,
      "newscategory": "(09/17) 56 ko",
      "newstitle_locstringid": -1,
      "newssubtitle_locstringid": -1,
      "newstext_locstringid": -1,
      "newsimage": "레드불 울롤로: 레거시 토너먼트 10월 21일 - 30일",
      "newsbody": "전투로! 레드불 울로로(Red Bull Wololo)가 돌아와 전 세계 최고의 Age of Empires 플레이어들을 모아 시대별 전투를 벌였습니다. TheViper가 타이틀을 방어할까요, 아니면 야심찬 경쟁자 중 한 명이 하이델베르크 성의 진정한 통치자로 선정될까요?\n\nRed Bull Wololo: Legacy는 10월 21일부터 10월 30일까지 운영됩니다. 대회의 모든 상황을 보려면 다음 채널을 확인하세요: twitch.tv/redbull.",
      "metadata": "NEWS;id=56;lang=ko",
      "datevisible": 1666386000,
      "expirytime": 1667196000
    },
    {
      "id": 831,
      "hidden": 0,
      "newscategory": "(10/17) 56 ms",
      "newstitle_locstringid": -1,
      "newssubtitle_locstringid": -1,
      "newstext_locstringid": -1,
      "newsimage": "Red Bull Wololo: Legacy Tournament 21 - 30 Oktober",
      "newsbody": "Ke medan peperangan! Red Bull Wololo kembali, menyatukan pemain Age of Empires terbaik dari seluruh dunia untuk pertempuran antara zaman. Adakah TheViper akan mempertahankan gelarannya, atau adakah pesaing yang bercita-cita tinggi akan dinobatkan sebagai pemerintah sebenar Kastil Heidelberg?\n\nRed Bull Wololo: Legacy berlangsung dari 21 Oktober hingga 30 Oktober. Ikuti di sini untuk menonton aksi: twitch.tv/redbull.",
      "metadata": "NEWS;id=56;lang=ms",
      "datevisible": 1666386000,
      "expirytime": 1667196000
    },
    {
      "id": 832,
      "hidden": 0,
      "newscategory": "(11/17) 56 br",
      "newstitle_locstringid": -1,
      "newssubtitle_locstringid": -1,
      "newstext_locstringid": -1,
      "newsimage": "",
      "newsbody": "",
      "metadata": "NEWS;id=56;lang=br",
      "datevisible": 1666386000,
      "expirytime": 1666591200
    },
    {
      "id": 833,
      "hidden": 0,
      "newscategory": "(12/17) 56 ru",
      "newstitle_locstringid": -1,
      "newssubtitle_locstringid": -1,
      "newstext_locstringid": -1,
      "newsimage": "Турнир Red Bull Wololo: Legacy 21–30 октября",
      "newsbody": "К оружию! Турнир Red Bull Wololo возвращается, чтобы лучшие игроки в Age of Empires со всего мира сошлись в битве века. Сможет ли TheViper защитить свой титул или кто-то из его соперников станет истинным правителем замка Heidelberg?\n\nТурнир Red Bull Wololo: Legacy будет проходить с 21 по 30 октября. Следите за обновлениями здесь: twitch.tv/redbull.",
      "metadata": "NEWS;id=56;lang=ru",
      "datevisible": 1666386000,
      "expirytime": 1667196000
    },
    {
      "id": 834,
      "hidden": 0,
      "newscategory": "(13/17) 56 es",
      "newstitle_locstringid": -1,
      "newssubtitle_locstringid": -1,
      "newstext_locstringid": -1,
      "newsimage": "Red Bull Wololo: Legacy Tournament del 21 al 30 de octubre",
      "newsbody": "¡A la batalla! Red Bull Wololo ha vuelto y está reuniendo a los mejores jugadores de Age of Empires de todo el mundo para una batalla histórica. ¿Defenderá TheViper su título o se coronará a uno de los competidores aspirantes como el verdadero gobernante del castillo de Heidelberg?\n\nRed Bull Wololo: Legacy se celebrará del 21 al 30 de octubre. Conéctate para no perderte la acción: twitch.tv/redbull.",
      "metadata": "NEWS;id=56;lang=es",
      "datevisible": 1666386000,
      "expirytime": 1667196000
    },
    {
      "id": 835,
      "hidden": 0,
      "newscategory": "(14/17) 56 mx",
      "newstitle_locstringid": -1,
      "newssubtitle_locstringid": -1,
      "newstext_locstringid": -1,
      "newsimage": "Red Bull Wololo: Legacy Tournament del 21 al 30 de octubre",
      "newsbody": "¡A la batalla! El torneo Red Bull Wololo está de vuelta para reunir a los mejores jugadores de Age of Empires de todo el mundo en una serie de batallas históricas. ¿Defenderá TheViper su título, o uno de los competidores le robará la corona y el trono del Castillo de Heidelberg?\n\nRed Bull Wololo: Legacy se celebra del 21 al 30 de octubre. Sintoniza aquí para vivir toda la acción: twitch.tv/redbull.",
      "metadata": "NEWS;id=56;lang=mx",
      "datevisible": 1666386000,
      "expirytime": 1667196000
    },
    {
      "id": 836,
      "hidden": 0,
      "newscategory": "(15/17) 56 tr",
      "newstitle_locstringid": -1,
      "newssubtitle_locstringid": -1,
      "newstext_locstringid": -1,
      "newsimage": "Red Bull Wololo: Legacy Turnuvası 21 - 30 Ekim",
      "newsbody": "Savaşa! Red Bull Wololo geri döndü ve dünyanın dört bir yanındaki en iyi Age of Empires oyuncularını çağlar boyu sürecek bir savaş için bir araya getirdi. TheViper unvanını koruyacak mı, yoksa hevesli rakiplerden biri Heidelberg Kalesi'nin gerçek hükümdarı olarak taçlandırılacak mı?\n\nRed Bull Wololo: Legacy, 21 Ekim'den 30 Ekim'e kadar sürecek. Bu kıyasıya mücadeleyi izlemek için bu adrese gel: twitch.tv/redbull.",
      "metadata": "NEWS;id=56;lang=tr",
      "datevisible": 1666386000,
      "expirytime": 1667196000
    },
    {
      "id": 837,
      "hidden": 0,
      "newscategory": "(16/17) 56 vi",
      "newstitle_locstringid": -1,
      "newssubtitle_locstringid": -1,
      "newstext_locstringid": -1,
      "newsimage": "Red Bull Wololo: Legacy Tournament 21 - 30 tháng 10",
      "newsbody": "Đã đến lúc chiến đấu! Red Bull Wololo đã trở lại, tập hợp những người chơi Age of Empires giỏi nhất từ khắp nơi trên thế giới để tham gia cuộc chiến thời đại. TheViper sẽ bảo vệ danh hiệu của mình, hay một trong những đối thủ cạnh tranh đầy tham vọng sẽ được trao vương miện người cai trị chân chính của Lâu đài Heidelberg?\n\nRed Bull Wololo: Legacy sẽ bắt đầu từ ngày 21 tháng 10 đến ngày 30 tháng 10. Hãy theo dõi tại đây để nắm bắt tất cả các tin tức mới nhất: twitch.tv/redbull.",
      "metadata": "NEWS;id=56;lang=vi",
      "datevisible": 1666386000,
      "expirytime": 1667196000
    },
    {
      "id": 838,
      "hidden": 0,
      "newscategory": "(17/17) 56 pl",
      "newstitle_locstringid": -1,
      "newssubtitle_locstringid": -1,
      "newstext_locstringid": -1,
      "newsimage": "Turniej Red Bull Wololo: Legacy 21-30 października",
      "newsbody": "Do walki! Red Bull Wololo powraca, gromadząc najlepszych graczy Age of Empires z całego świata na epokową bitwę. Czy TheViper obroni swój tytuł, czy może jeden z aspirujących zawodników zostanie koronowany na prawdziwego władcę zamku Heidelberg?\n\nRed Bull Wololo: Legacy trwa od 21 do 30 października. Dołącz tutaj, aby niczego nie przegapić: twitch.tv/redbull.",
      "metadata": "NEWS;id=56;lang=pl",
      "datevisible": 1666386000,
      "expirytime": 1667196000
    },
    {
      "id": 811,
      "hidden": 0,
      "newscategory": "",
      "newstitle_locstringid": 31,
      "newssubtitle_locstringid": -1,
      "newstext_locstringid": 32,
      "newsimage": "NEW DLC AVAILABLE NOW: Dynasties of India!",
      "newsbody": "DYNASTIES OF INDIA is Live!\r\n\r\nThe latest DLC for Age of Empires II: Definitive Edition remixes the previous Indian Civ (now the Hindustani) and introduces THREE new Civilizations - the Dravidians, the Bengalis, and the Gurjaras! \r\n\r\nThis expansion includes three all-NEW Campaigns that explore the rich history of India, alongside new units and tactics bound to shake up your MP games! Did somebody say Elephants?",
      "metadata": "LNEWS;PROMOTION=DLC_PORTO;",
      "datevisible": 1651161600,
      "expirytime": 1714233600
    },
    {
      "id": 1,
      "hidden": 0,
      "newscategory": "",
      "newstitle_locstringid": 1,
      "newssubtitle_locstringid": -1,
      "newstext_locstringid": 2,
      "newsimage": "Welcome to Age of Empires II: Definitive Edition!",
      "newsbody": "Welcome to Age of Empires II: Definitive Edition! We are excited to have you join us for the launch of the game, and look forward to building a legacy that will stand the test of time and continue to grow in the years to come!\r\n\r\nAs you begin your journey, take the time to follow our social channels for news, updates, and information about what we have in store for Age of Empires:. If you encounter an issue while playing, you can visit ageofempires.com/support for troubleshooting tips and common solutions.\r\n\r\nWe hope you enjoy the Definitive Edition, and encourage you to come talk with us about your experience, leave us feedback, and let us know of any issues you encounter in the game.\r\n\r\nThank you for playing!\r\n\r\n- The Age of Empires Team",
      "metadata": "LNEWS",
      "datevisible": 1573660800,
      "expirytime": 1763064000
    }
  ]
}
```

```
{
    "$schema": "http://json-schema.org/schema#",
    "type": "object",
    "properties": {
        "result": {
            "type": "object",
            "properties": {
                "code": {
                    "type": "integer"
                },
                "message": {
                    "type": "string"
                }
            },
            "required": [
                "code",
                "message"
            ]
        },
        "news": {
            "type": "array",
            "items": {
                "type": "object",
                "properties": {
                    "id": {
                        "type": "integer"
                    },
                    "hidden": {
                        "type": "integer"
                    },
                    "newscategory": {
                        "type": "string"
                    },
                    "newstitle_locstringid": {
                        "type": "integer"
                    },
                    "newssubtitle_locstringid": {
                        "type": "integer"
                    },
                    "newstext_locstringid": {
                        "type": "integer"
                    },
                    "newsimage": {
                        "type": "string"
                    },
                    "newsbody": {
                        "type": "string"
                    },
                    "metadata": {
                        "type": "string"
                    },
                    "datevisible": {
                        "type": "integer"
                    },
                    "expirytime": {
                        "type": "integer"
                    }
                },
                "required": [
                    "datevisible",
                    "expirytime",
                    "hidden",
                    "id",
                    "metadata",
                    "newsbody",
                    "newscategory",
                    "newsimage",
                    "newssubtitle_locstringid",
                    "newstext_locstringid",
                    "newstitle_locstringid"
                ]
            }
        }
    },
    "required": [
        "news",
        "result"
    ]
}
```
