<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>My Nouns 🇺🇸 — تعلّم الأسماء الإنجليزية</title>
<style>
*{box-sizing:border-box;margin:0;padding:0;-webkit-tap-highlight-color:transparent}
body{font-family:'Segoe UI',Tahoma,system-ui,sans-serif;background:linear-gradient(135deg,#667eea,#764ba2);min-height:100vh;padding-bottom:90px;color:#1a1a2e;overflow-x:hidden}
header{background:rgba(255,255,255,.97);padding:14px 16px;text-align:center;box-shadow:0 2px 12px rgba(0,0,0,.12);position:sticky;top:0;z-index:100}
header h1{font-size:1.25rem;color:#4a3f8f;display:flex;align-items:center;justify-content:center;gap:8px}
header p{font-size:.78rem;color:#777;margin-top:3px}
.searchbar{margin-top:10px;position:relative}
.searchbar input{width:100%;padding:11px 42px 11px 16px;border:2px solid #e0e0f0;border-radius:30px;font-size:.95rem;outline:none;transition:.2s;background:#f8f8ff}
.searchbar input:focus{border-color:#764ba2;background:#fff}
.searchbar::before{content:'🔎';position:absolute;right:15px;top:50%;transform:translateY(-50%);font-size:1rem}
main{padding:14px}
.grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(140px,1fr));gap:10px}
.card{background:#fff;border-radius:16px;padding:12px;box-shadow:0 3px 10px rgba(0,0,0,.09);cursor:pointer;transition:.18s;text-align:center;position:relative;overflow:hidden}
.card:active{transform:scale(.96)}
.card .emo{font-size:2.4rem;display:block;line-height:1.3}
.card .en{font-weight:700;color:#4a3f8f;font-size:.95rem;margin-top:4px;word-break:break-word}
.card .ar{font-size:.78rem;color:#888;margin-top:2px}
.card .fav{position:absolute;top:6px;left:8px;font-size:1rem;opacity:.35}
.card .fav.on{opacity:1}
.detail{background:#fff;border-radius:22px;padding:20px;box-shadow:0 8px 28px rgba(0,0,0,.15);animation:pop .25s ease}
@keyframes pop{from{transform:scale(.94);opacity:0}to{transform:scale(1);opacity:1}}
.back{background:#f0f0ff;border:none;padding:8px 16px;border-radius:20px;cursor:pointer;font-size:.85rem;color:#4a3f8f;font-weight:600;margin-bottom:14px}
.imgbox{background:linear-gradient(135deg,#e8ecff,#f8e8ff);border-radius:20px;height:150px;display:flex;align-items:center;justify-content:center;font-size:5rem;margin-bottom:14px}
.word-en{font-size:2rem;font-weight:800;color:#4a3f8f;text-align:center;letter-spacing:.5px}
.word-ar{font-size:1.15rem;color:#666;text-align:center;margin-top:4px}
.row{display:flex;gap:8px;margin-top:16px;flex-wrap:wrap}
.btn{flex:1;min-width:100px;padding:12px;border:none;border-radius:14px;font-size:.9rem;font-weight:600;cursor:pointer;transition:.15s;display:flex;align-items:center;justify-content:center;gap:6px}
.btn:active{transform:scale(.96)}
.btn-primary{background:linear-gradient(135deg,#667eea,#764ba2);color:#fff}
.btn-ghost{background:#f0f0ff;color:#4a3f8f}
.btn-fav{background:#ffe8f0;color:#e91e63}
.btn-fav.on{background:#e91e63;color:#fff}
.example{background:#f8f8ff;border-radius:14px;padding:14px;margin-top:16px;border-right:4px solid #764ba2}
.example .ex-en{font-size:.95rem;color:#333;font-weight:600;direction:ltr;text-align:left}
.example .ex-ar{font-size:.85rem;color:#777;margin-top:6px}
.mic-status{margin-top:12px;text-align:center;font-size:.85rem;min-height:22px;font-weight:600}
.mic-status.good{color:#2e7d32}.mic-status.mid{color:#f57c00}.mic-status.bad{color:#c62828}
.list-view{background:#fff;border-radius:18px;padding:16px;box-shadow:0 4px 16px rgba(0,0,0,.1)}
.list-view h2{color:#4a3f8f;font-size:1.05rem;margin-bottom:12px;display:flex;align-items:center;gap:8px}
.chatbox{background:#fff;border-radius:18px;padding:14px;box-shadow:0 4px 16px rgba(0,0,0,.1);height:calc(100vh - 250px);display:flex;flex-direction:column}
.chat-msgs{flex:1;overflow-y:auto;padding:6px;display:flex;flex-direction:column;gap:10px}
.msg{max-width:82%;padding:10px 14px;border-radius:16px;font-size:.9rem;line-height:1.5;animation:pop .2s}
.msg.bot{background:#f0f0ff;color:#333;align-self:flex-start;border-bottom-right-radius:4px}
.msg.user{background:linear-gradient(135deg,#667eea,#764ba2);color:#fff;align-self:flex-end;border-bottom-left-radius:4px}
.chat-input{display:flex;gap:8px;margin-top:10px}
.chat-input input{flex:1;padding:11px 14px;border:2px solid #e0e0f0;border-radius:22px;font-size:.9rem;outline:none}
.chat-input input:focus{border-color:#764ba2}
.chat-input button{background:linear-gradient(135deg,#667eea,#764ba2);color:#fff;border:none;border-radius:50%;width:44px;height:44px;font-size:1.1rem;cursor:pointer}
nav{position:fixed;bottom:0;right:0;left:0;background:#fff;display:flex;box-shadow:0 -3px 14px rgba(0,0,0,.1);z-index:100;padding:6px 0}
nav button{flex:1;background:none;border:none;padding:8px 4px;cursor:pointer;display:flex;flex-direction:column;align-items:center;gap:3px;font-size:.7rem;color:#999;font-weight:600;transition:.2s}
nav button .ic{font-size:1.35rem}
nav button.active{color:#764ba2}
nav button.active .ic{transform:scale(1.15)}
.stat{display:grid;grid-template-columns:1fr 1fr;gap:12px;margin-bottom:14px}
.stat-card{background:#fff;border-radius:16px;padding:16px;text-align:center;box-shadow:0 3px 10px rgba(0,0,0,.08)}
.stat-card .num{font-size:2rem;font-weight:800;color:#764ba2}
.stat-card .lbl{font-size:.78rem;color:#888;margin-top:4px}
.progress-bar{height:10px;background:#eee;border-radius:10px;overflow:hidden;margin-top:8px}
.progress-bar div{height:100%;background:linear-gradient(90deg,#667eea,#764ba2);border-radius:10px;transition:.4s}
.empty{text-align:center;padding:40px 20px;color:#999}
.empty .ic{font-size:3rem;display:block;margin-bottom:10px}
.hidden{display:none!important}
.add-form{background:#fff;border-radius:18px;padding:16px;margin-top:14px;box-shadow:0 4px 16px rgba(0,0,0,.1)}
.add-form h3{color:#4a3f8f;font-size:.95rem;margin-bottom:10px}
.add-form input,.add-form textarea{width:100%;padding:9px 12px;border:2px solid #e0e0f0;border-radius:12px;font-size:.85rem;outline:none;margin-bottom:8px;font-family:inherit}
.add-form input:focus,.add-form textarea:focus{border-color:#764ba2}
.chip{display:inline-block;background:#f0f0ff;color:#4a3f8f;padding:6px 12px;border-radius:14px;font-size:.75rem;margin:3px;cursor:pointer;font-weight:600}
</style>
</head>
<body>

<header>
  <h1>🇺🇸 My Nouns</h1>
  <p>تعلّم الأسماء الإنجليزية الأمريكية</p>
  <div class="searchbar">
    <input id="search" type="text" placeholder="ابحث عن كلمة بالعربية أو الإنجليزية...">
  </div>
</header>

<main id="app"></main>

<nav>
  <button data-nav="words" class="active"><span class="ic">📚</span>الكلمات</button>
  <button data-nav="favorites"><span class="ic">❤️</span>المفضلة</button>
  <button data-nav="chat"><span class="ic">🤖</span>محادثة AI</button>
  <button data-nav="progress"><span class="ic">📊</span>تقدمي</button>
</nav>

<script>
/* ==================== قاعدة الكلمات ==================== */
const RAW = [
/* حيوانات */
['cat','قطة','The cat is sleeping on the sofa.','القطة نائمة على الأريكة.','🐱'],
['dog','كلب','My dog likes to play in the yard.','كلبي يحب اللعب في الفناء.','🐶'],
['bird','طائر','The bird sings in the morning.','الطائر يغني في الصباح.','🐦'],
['fish','سمكة','The fish swims in the water.','السمكة تسبح في الماء.','🐟'],
['horse','حصان','The horse runs very fast.','الحصان يركض بسرعة كبيرة.','🐴'],
['cow','بقرة','The cow gives us milk.','البقرة تعطينا الحليب.','🐮'],
['sheep','خروف','The sheep is white and soft.','الخروف أبيض وناعم.','🐑'],
['lion','أسد','The lion is the king of animals.','الأسد ملك الحيوانات.','🦁'],
['tiger','نمر','The tiger has black stripes.','النمر لديه خطوط سوداء.','🐯'],
['elephant','فيل','The elephant is very big.','الفيل كبير جداً.','🐘'],
['monkey','قرد','The monkey climbs the tall tree.','القرد يتسلق الشجرة العالية.','🐵'],
['rabbit','أرنب','The rabbit eats a carrot.','الأرنب يأكل جزرة.','🐰'],
['mouse','فأر','The mouse is very small.','الفأر صغير جداً.','🐭'],
['bear','دب','The bear lives in the forest.','الدب يعيش في الغابة.','🐻'],
['wolf','ذئب','The wolf howls at night.','الذئب يعوي في الليل.','🐺'],
['snake','ثعبان','The snake is very long.','الثعبان طويل جداً.','🐍'],
['frog','ضفدع','The frog jumps high.','الضفدع يقفز عالياً.','🐸'],
['duck','بطة','The duck swims in the pond.','البطة تسبح في البركة.','🦆'],
['chicken','دجاجة','The chicken lays eggs.','الدجاجة تضع البيض.','🐔'],
['bee','نحلة','The bee makes sweet honey.','النحلة تصنع عسلاً حلواً.','🐝'],
/* طعام */
['apple','تفاحة','I eat an apple every day.','آكل تفاحة كل يوم.','🍎'],
['banana','موزة','The banana is yellow.','الموزة صفراء.','🍌'],
['orange','برتقالة','The orange is very juicy.','البرتقالة كثيرة العصير.','🍊'],
['bread','خبز','I eat bread for breakfast.','آكل الخبز في الفطور.','🍞'],
['milk','حليب','I drink milk in the morning.','أشرب الحليب في الصباح.','🥛'],
['water','ماء','I drink cold water.','أشرب ماءً بارداً.','💧'],
['rice','أرز','We eat rice with chicken.','نأكل الأرز مع الدجاج.','🍚'],
['meat','لحم','The meat is on the plate.','اللحم على الطبق.','🥩'],
['egg','بيضة','I eat an egg for breakfast.','آكل بيضة في الفطور.','🥚'],
['cheese','جبن','I like cheese on bread.','أحب الجبن على الخبز.','🧀'],
['butter','زبدة','She puts butter on the toast.','تضع الزبدة على الخبز المحمص.','🧈'],
['sugar','سكر','I add sugar to my tea.','أضيف السكر إلى شايي.','🍬'],
['salt','ملح','The soup needs more salt.','الحساء يحتاج مزيداً من الملح.','🧂'],
['coffee','قهوة','I drink coffee in the morning.','أشرب القهوة في الصباح.','☕'],
['tea','شاي','She likes green tea.','تحب الشاي الأخضر.','🍵'],
['juice','عصير','The orange juice is fresh.','عصير البرتقال طازج.','🧃'],
['cake','كعكة','We eat cake on birthdays.','نأكل الكعكة في أعياد الميلاد.','🍰'],
['chocolate','شوكولاتة','I love dark chocolate.','أحب الشوكولاتة الداكنة.','🍫'],
['pizza','بيتزا','We ordered a big pizza.','طلبنا بيتزا كبيرة.','🍕'],
['sandwich','شطيرة','I made a cheese sandwich.','صنعت شطيرة جبن.','🥪'],
['salad','سلطة','The salad is fresh and healthy.','السلطة طازجة وصحية.','🥗'],
['soup','حساء','The soup is very hot.','الحساء ساخن جداً.','🍲'],
['fruit','فاكهة','Fruit is good for health.','الفاكهة مفيدة للصحة.','🍇'],
['vegetable','خضار','Eat your vegetables every day.','كل خضارك كل يوم.','🥦'],
['honey','عسل','Honey is very sweet.','العسل حلو جداً.','🍯'],
/* منزل */
['house','منزل','This is my new house.','هذا منزلي الجديد.','🏠'],
['room','غرفة','My room is clean and tidy.','غرفتي نظيفة ومرتبة.','🛏️'],
['door','باب','Please close the door.','أغلق الباب من فضلك.','🚪'],
['window','نافذة','Open the window, please.','افتح النافذة من فضلك.','🪟'],
['wall','جدار','The wall is painted white.','الجدار مطلي باللون الأبيض.','🧱'],
['floor','أرضية','The floor is very clean.','الأرضية نظيفة جداً.','🟫'],
['roof','سقف','The roof is painted red.','السقف مطلي بالأحمر.','🛖'],
['kitchen','مطبخ','Mom cooks in the kitchen.','أمي تطبخ في المطبخ.','🍳'],
['bedroom','غرفة نوم','I sleep in my bedroom.','أنام في غرفة نومي.','🛌'],
['bathroom','حمام','The bathroom is very small.','الحمام صغير جداً.','🚿'],
['table','طاولة','The book is on the table.','الكتاب على الطاولة.','🍽️'],
['chair','كرسي','Sit on the wooden chair.','اجلس على الكرسي الخشبي.','🪑'],
['bed','سرير','The bed is very comfortable.','السرير مريح جداً.','🛏️'],
['sofa','أريكة','We sit on the sofa together.','نجلس على الأريكة معاً.','🛋️'],
['lamp','مصباح','Turn on the lamp, please.','شغّل المصباح من فضلك.','💡'],
['mirror','مرآة','She looks in the mirror.','تنظر في المرآة.','🪞'],
['clock','ساعة حائط','The clock is on the wall.','الساعة على الجدار.','🕐'],
['key','مفتاح','I lost my house key.','فقدت مفتاح منزلي.','🔑'],
['cup','كوب','I drink tea from the cup.','أشرب الشاي من الكوب.','🥤'],
['plate','طبق','The plate is empty now.','الطبق فارغ الآن.','🍽️'],
/* جسم */
['head','رأس','My head hurts a little.','رأسي يؤلمني قليلاً.','👤'],
['eye','عين','She has beautiful blue eyes.','لديها عيون زرقاء جميلة.','👁️'],
['ear','أذن','I hear with my ear.','أسمع بأذني.','👂'],
['nose','أنف','The nose is in the middle.','الأنف في الوسط.','👃'],
['mouth','فم','Open your mouth, please.','افتح فمك من فضلك.','👄'],
['tooth','سن','Brush your teeth every day.','نظّف أسنانك كل يوم.','🦷'],
['hand','يد','Give me your hand.','أعطني يدك.','✋'],
['foot','قدم','My foot is a little cold.','قدمي باردة قليلاً.','🦶'],
['arm','ذراع','He broke his right arm.','كسر ذراعه اليمنى.','💪'],
['leg','ساق','The leg is long and strong.','الساق طويلة وقوية.','🦵'],
['hair','شعر','Her hair is long and black.','شعرها طويل وأسود.','💇'],
['face','وجه','Wash your face with water.','اغسل وجهك بالماء.','😊'],
['finger','إصبع','I have ten fingers.','لدي عشرة أصابع.','👆'],
['heart','قلب','The heart beats day and night.','القلب ينبض ليلاً ونهاراً.','❤️'],
['back','ظهر','My back hurts from sitting.','ظهري يؤلمني من الجلوس.','🧍'],
/* طبيعة */
['sun','شمس','The sun is bright today.','الشمس مشرقة اليوم.','☀️'],
['moon','قمر','The moon shines at night.','القمر يضيء في الليل.','🌙'],
['star','نجمة','The stars are in the sky.','النجوم في السماء.','⭐'],
['sky','سماء','The sky is blue today.','السماء زرقاء اليوم.','🌌'],
['cloud','سحابة','The cloud is big and white.','السحابة كبيرة وبيضاء.','☁️'],
['rain','مطر','The rain is very heavy.','المطر غزير جداً.','🌧️'],
['snow','ثلج','The snow is cold and white.','الثلج بارد وأبيض.','❄️'],
['wind','ريح','The wind is strong today.','الريح قوية اليوم.','🌬️'],
['fire','نار','The fire is very hot.','النار ساخنة جداً.','🔥'],
['tree','شجرة','The tree is tall and old.','الشجرة طويلة وقديمة.','🌳'],
['flower','زهرة','The flower is very beautiful.','الزهرة جميلة جداً.','🌸'],
['grass','عشب','The grass is green and wet.','العشب أخضر ومبلل.','🌿'],
['mountain','جبل','The mountain is very high.','الجبل مرتفع جداً.','🏔️'],
['river','نهر','The river is long and wide.','النهر طويل وعريض.','🏞️'],
['sea','بحر','The sea is deep and blue.','البحر عميق وأزرق.','🌊'],
['beach','شاطئ','We play on the sandy beach.','نلعب على الشاطئ الرملي.','🏖️'],
['stone','حجر','The stone is hard and heavy.','الحجر صلب وثقيل.','🪨'],
['sand','رمل','The sand is warm in summer.','الرمل دافئ في الصيف.','⏳'],
['leaf','ورقة شجر','The leaf is green and small.','الورقة خضراء وصغيرة.','🍃'],
['seed','بذرة','Plant the seed in the soil.','ازرع البذرة في التراب.','🌱'],
/* أشخاص */
['man','رجل','The man is very tall.','الرجل طويل جداً.','👨'],
['woman','امرأة','The woman is kind and gentle.','المرأة طيبة ولطيفة.','👩'],
['boy','ولد','The boy plays football well.','الولد يلعب كرة القدم جيداً.','👦'],
['girl','بنت','The girl reads a story.','البنت تقرأ قصة.','👧'],
['child','طفل','The child is very happy.','الطفل سعيد جداً.','🧒'],
['baby','رضيع','The baby is sleeping now.','الرضيع نائم الآن.','👶'],
['father','أب','My father works very hard.','أبي يعمل بجد كبير.','👨‍🦱'],
['mother','أم','My mother cooks delicious food.','أمي تطبخ طعاماً لذيذاً.','👩‍🦰'],
['brother','أخ','My brother is still young.','أخي ما زال صغيراً.','🧑'],
['sister','أخت','My sister is very smart.','أختي ذكية جداً.','👩‍🦱'],
['friend','صديق','He is my best friend.','هو أفضل صديق لي.','🤝'],
['teacher','معلم','The teacher explains the lesson.','المعلم يشرح الدرس.','👨‍🏫'],
['doctor','طبيب','The doctor helps sick people.','الطبيب يساعد المرضى.','👨‍⚕️'],
['student','طالب','The student studies every night.','الطالب يدرس كل ليلة.','🧑‍🎓'],
['family','عائلة','My family is big and happy.','عائلتي كبيرة وسعيدة.','👨‍👩‍👧‍👦'],
/* أماكن */
['school','مدرسة','I go to school by bus.','أذهب إلى المدرسة بالحافلة.','🏫'],
['hospital','مستشفى','The hospital is very big.','المستشفى كبير جداً.','🏥'],
['market','سوق','We buy food at the market.','نشتري الطعام من السوق.','🏪'],
['park','حديقة عامة','The kids play in the park.','الأطفال يلعبون في الحديقة.','🌳'],
['city','مدينة','The city is busy and loud.','المدينة مزدحمة وصاخبة.','🏙️'],
['village','قرية','The village is quiet and small.','القرية هادئة وصغيرة.','🏘️'],
['street','شارع','The street is long and wide.','الشارع طويل وعريض.','🛣️'],
['road','طريق','The road is narrow here.','الطريق ضيق هنا.','🛤️'],
['bank','بنك','I go to the bank today.','أذهب إلى البنك اليوم.','🏦'],
['hotel','فندق','We stayed at a nice hotel.','مكثنا في فندق جميل.','🏨'],
['restaurant','مطعم','The restaurant is very full.','المطعم ممتلئ جداً.','🍴'],
['airport','مطار','The airport is far from here.','المطار بعيد من هنا.','✈️'],
['station','محطة','The train station is near.','محطة القطار قريبة.','🚉'],
['library','مكتبة','The library is very quiet.','المكتبة هادئة جداً.','📚'],
['museum','متحف','We visited the old museum.','زرنا المتحف القديم.','🏛️'],
/* أشياء */
['book','كتاب','I read an interesting book.','أقرأ كتاباً ممتعاً.','📖'],
['pen','قلم حبر','Write with a blue pen.','اكتب بقلم أزرق.','🖊️'],
['pencil','قلم رصاص','Use a pencil for drawing.','استخدم قلم الرصاص للرسم.','✏️'],
['paper','ورقة','I need a clean paper.','أحتاج ورقة نظيفة.','📄'],
['bag','حقيبة','My bag is very heavy.','حقيبتي ثقيلة جداً.','🎒'],
['phone','هاتف','My phone is brand new.','هاتفي جديد تماماً.','📱'],
['computer','حاسوب','I work on my computer.','أعمل على حاسوبي.','💻'],
['car','سيارة','The car is very fast.','السيارة سريعة جداً.','🚗'],
['bus','حافلة','I take the bus to work.','أستقل الحافلة إلى العمل.','🚌'],
['train','قطار','The train is late today.','القطار متأخر اليوم.','🚆'],
['bike','دراجة','I ride my bike in the park.','أركب دراجتي في الحديقة.','🚲'],
['plane','طائرة','The plane flies very high.','الطائرة تطير عالياً جداً.','🛫'],
['ship','سفينة','The ship is huge and white.','السفينة ضخمة وبيضاء.','🚢'],
['shirt','قميص','He wears a blue shirt.','يلبس قميصاً أزرق.','👕'],
['shoe','حذاء','My shoes are very new.','حذائي جديد جداً.','👟'],
['hat','قبعة','She wears a red hat.','تلبس قبعة حمراء.','🎩'],
['watch','ساعة يد','My watch is old but works.','ساعتي قديمة لكنها تعمل.','⌚'],
['glasses','نظارات','I need my glasses to read.','أحتاج نظاراتي للقراءة.','👓'],
['money','مال','I have no money today.','ليس لدي مال اليوم.','💰'],
['gift','هدية','This is a gift for you.','هذه هدية لك.','🎁'],
/* وقت */
['day','يوم','Today is a beautiful day.','اليوم يوم جميل.','📅'],
['night','ليل','The night is quiet and calm.','الليل هادئ وساكن.','🌃'],
['morning','صباح','Good morning, my friend!','صباح الخير يا صديقي!','🌅'],
['evening','مساء','Good evening, everyone!','مساء الخير للجميع!','🌆'],
['week','أسبوع','The week has seven days.','الأسبوع سبعة أيام.','📆'],
['month','شهر','This month is very short.','هذا الشهر قصير جداً.','🗓️'],
['year','سنة','Happy New Year to you!','سنة جديدة سعيدة لك!','🎆'],
['hour','ساعة','Wait for one hour only.','انتظر ساعة واحدة فقط.','⏰'],
['minute','دقيقة','Wait a minute, please.','انتظر دقيقة من فضلك.','⏱️'],
['today','اليوم','Today is Monday.','اليوم هو الاثنين.','📌'],
/* معاني */
['love','حب','Love is a beautiful feeling.','الحب شعور جميل.','💖'],
['hope','أمل','Never lose hope in life.','لا تفقد الأمل في الحياة.','🌟'],
['dream','حلم','I have a big dream.','لدي حلم كبير.','💭'],
['idea','فكرة','That is a great idea!','هذه فكرة رائعة!','🧠'],
['question','سؤال','I have an important question.','لدي سؤال مهم.','❓'],
['answer','جواب','The answer is correct.','الجواب صحيح.','✅'],
['word','كلمة','Learn one word every day.','تعلّم كلمة كل يوم.','🔤'],
['name','اسم','What is your name?','ما اسمك؟','🏷️'],
['number','رقم','Pick a number from one to ten.','اختر رقماً من واحد إلى عشرة.','🔢'],
['color','لون','What is your favorite color?','ما لونك المفضل؟','🎨'],
['music','موسيقى','I love calm music.','أحب الموسيقى الهادئة.','🎵'],
['story','قصة','Tell me a short story.','اخبرني قصة قصيرة.','📜'],
['game','لعبة','Let us play a fun game.','هيا نلعب لعبة ممتعة.','🎮'],
['work','عمل','I go to work every day.','أذهب إلى العمل كل يوم.','💼'],
['life','حياة','Life is short and precious.','الحياة قصيرة وثمينة.','🌈'],
/* إضافات */
['garden','حديقة منزل','The garden is full of flowers.','الحديقة مليئة بالزهور.','🌷'],
['bridge','جسر','The bridge is old and long.','الجسر 
