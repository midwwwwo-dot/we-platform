<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>منصة المصري لمدارس We للتكنولوجيا التطبيقية</title>
<link rel="manifest" href="data:application/json,[STRIPPED] المصري&quot;,&quot;short_name&quot;:&quot;منصة المصري&quot;,&quot;start_url&quot;:&quot;.&quot;,&quot;display&quot;:&quot;standalone&quot;,&quot;background_color&quot;:&quot;#0057b8&quot;,&quot;theme_color&quot;:&quot;#0057b8&quot;,&quot;icons&quot;:[{&quot;src&quot;:&quot;data:image/svg+xml;base64,[STRIPPED]&quot;,&quot;sizes&quot;:&quot;512x512&quot;}]}">
<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:Tahoma,Arial,sans-serif}
body{background:#f0f8ff;overflow-x:hidden}
.header{background:linear-gradient(135deg,#7c3aed 0%,#f97316 100%);padding:12px 20px;display:flex;align-items:center;justify-content:space-between;color:#fff;box-shadow:0 4px 12px rgba(0,0,0,0.2)}
.logo{display:flex;align-items:center;gap:12px}
.logo-circle{width:48px;height:48px;background:#fff;border-radius:50%;display:flex;align-items:center;justify-content:center;font-weight:900;color:#ff6b00;font-size:20px;cursor:pointer}
.header h1{font-size:18px;font-weight:700}
.header-icons{display:flex;gap:16px}
.icon-btn{width:40px;height:40px;background:rgba(255,255,255,0.2);border-radius:50%;border:none;cursor:pointer;display:flex;align-items:center;justify-content:center;font-size:20px}
.hero{background:linear-gradient(180deg,#b3e5fc 0%,#81d4fa 100%);padding:30px 20px 0;position:relative;min-height:320px}
.hero-bg{position:absolute;inset:0;overflow:hidden}
.sun{position:absolute;top:20px;left:30px;width:80px;height:80px;background:#ffeb3b;border-radius:50%;box-shadow:0 0 40px #ffeb3b}
.tree{position:absolute;bottom:0;right:40px;width:120px;height:160px}
.mountain{position:absolute;bottom:60px;left:0;right:0;height:100px;background:#90caf9;clip-path:polygon(0 100%, 15% 40%, 25% 60%, 35% 30%, 50% 70%, 65% 35%, 75% 55%, 90% 40%, 100% 100%)}
.sea{position:absolute;bottom:0;left:0;right:0;height:60px;background:#4fc3f7}
.boat{position:absolute;bottom:70px;left:50%;width:40px;height:30px}
.students{position:absolute;bottom:10px;right:20px;display:flex;gap:10px;z-index:10}
.student{width:70px;height:90px}
.hero-content{position:relative;z-index:5;text-align:right;padding-right:20px}
.hero-content h2{font-size:32px;color:#01579b;margin-bottom:10px;font-weight:900}
.hero-content p{font-size:16px;color:#0277bd;margin-bottom:8px}
.section-title{text-align:center;padding:30px 20px;font-size:28px;font-weight:900;color:#1a237e}
.grades{display:grid;grid-template-columns:repeat(auto-fit,minmax(300px,1fr));gap:24px;padding:20px;max-width:1200px;margin:0 auto}
.grade-card{border-radius:24px;padding:24px;box-shadow:0 8px 24px rgba(0,0,0,0.15);cursor:pointer;transition:transform 0.3s;border:4px solid rgba(255,255,255,0.5);position:relative}
.grade-card:hover{transform:translateY(-8px);box-shadow:0 12px 32px rgba(0,0,0,0.25)}
.grade-card.orange{background:linear-gradient(135deg,#ff9800 0%,#f57c00 100%)}
.grade-card.blue{background:linear-gradient(135deg,#2196f3 0%,#1976d2 100%)}
.grade-card.yellow{background:linear-gradient(135deg,#ffc107 0%,#ffa000 100%)}
.grade-icon{width:80px;height:80px;background:rgba(255,255,255,0.3);border-radius:20px;margin:0 auto 16px;display:flex;align-items:center;justify-content:center;font-size:48px}
.grade-card h3{font-size:26px;color:#fff;text-align:center;margin-bottom:12px;font-weight:900}
.grade-card p{color:#fff;text-align:center;font-size:14px;margin-bottom:8px;line-height:1.6}
.grade-tag{background:rgba(0,0,0,0.2);padding:8px 16px;border-radius:12px;color:#fff;font-size:13px;text-align:center;margin:12px 0}
.grade-btn{background:#fff;color:#333;border:none;padding:14px 32px;border-radius:16px;font-weight:700;font-size:16px;cursor:pointer;width:100%;margin-top:12px}
.stats{background:#e3f2fd;padding:30px 20px;display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:16px}
.stat-card{background:#fff;border-radius:16px;padding:20px;text-align:center;box-shadow:0 4px 12px rgba(0,0,0,0.1)}
.stat-icon{font-size:40px;margin-bottom:8px}
.stat-card h4{font-size:14px;color:#546e7a;margin-bottom:4px}
.footer{background:#263238;color:#fff;text-align:center;padding:20px;font-size:14px}
.page{display:none;padding:20px;max-width:1200px;margin:0 auto}
.page.active{display:block}
.back-btn{background:#546e7a;color:#fff;border:none;padding:12px 24px;border-radius:12px;cursor:pointer;margin-bottom:20px;font-size:16px}
.books-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(280px,1fr));gap:20px;margin-top:20px}
.book-card{background:#fff;border-radius:16px;padding:20px;box-shadow:0 4px 12px rgba(0,0,0,0.1);cursor:pointer;transition:transform 0.2s}
.book-card:hover{transform:translateY(-4px)}
.book-icon{font-size:48px;text-align:center;margin-bottom:12px}
.book-card h4{font-size:18px;margin-bottom:8px;color:#1a237e}
.book-card p{font-size:13px;color:#546e7a}
.lesson-view{background:#fff;border-radius:16px;padding:30px;margin-top:20px}
.lesson-text{font-size:20px;line-height:2.2;color:#263238;margin:20px 0}
.controls{display:flex;gap:12px;flex-wrap:wrap;margin:20px 0}
.ctrl-btn{background:#2196f3;color:#fff;border:none;padding:12px 20px;border-radius:12px;cursor:pointer;font-size:16px}
.ctrl-btn:hover{background:#1976d2}
.install-btn{position:fixed;top:80px;left:20px;background:#4caf50;color:#fff;border:none;padding:14px 24px;border-radius:12px;font-weight:700;cursor:pointer;z-index:1000;box-shadow:0 4px 12px rgba(0,0,0,0.3)}
.admin-panel{background:#fff3e0;padding:20px;border-radius:16px;margin:20px 0;display:none}
.admin-panel.active{display:block}
input,textarea,select{width:100%;padding:12px;border:2px solid #b0bec5;border-radius:8px;margin:8px 0;font-size:16px;font-family:inherit}
textarea{min-height:150px}
</style>
</head>
<body>
<button class="install-btn" id="installBtn" style="display:none">📱 تثبيت التطبيق</button>

<div id="mainPage">
<header class="header">
<div class="logo">
<div class="logo-circle" id="logoClick">We</div>
<h1>منصة المصري لمدارس We للتكنولوجيا التطبيقية</h1>
</div>
<div class="header-icons">
<button class="icon-btn">🔔</button>
<button class="icon-btn">👤</button>
<button class="icon-btn">⚙️</button>
</div>
</header>

<section class="hero">
<div class="hero-bg">
<div class="sun"></div>
<svg class="tree" viewBox="0 0 120 160"><rect x="50" y="80" width="20" height="80" fill="#6d4c41"/><circle cx="60" cy="60" r="40" fill="#4caf50"/><circle cx="40" cy="70" r="30" fill="#66bb6a"/><circle cx="80" cy="70" r="30" fill="#66bb6a"/></svg>
<div class="mountain"></div>
<div class="sea"></div>
<svg class="boat" viewBox="0 0 40 30"><polygon points="20,5 35,25 5,25" fill="#ff6f00"/><rect x="18" y="0" width="4" height="15" fill="#8d6e63"/></svg>
</div>
<div class="students">
<svg class="student" viewBox="0 0 70 90"><circle cx="35" cy="20" r="15" fill="#ffcc80"/><rect x="20" y="35" width="30" height="35" rx="5" fill="#2196f3"/><rect x="15" y="45" width="12" height="25" rx="6" fill="#ffcc80"/><rect x="43" y="45" width="12" height="25" rx="6" fill="#ffcc80"/><rect x="22" y="70" width="10" height="20" fill="#1565c0"/><rect x="38" y="70" width="10" height="20" fill="#1565c0"/><rect x="25" y="55" width="20" height="15" rx="3" fill="#90caf9"/></svg>
<svg class="student" viewBox="0 0 70 90"><circle cx="35" cy="20" r="15" fill="#ffcc80"/><path d="M 20 20 Q 35 10 50 20 L 50 35 Q 35 30 20 35 Z" fill="#e91e63"/><rect x="20" y="35" width="30" height="35" rx="5" fill="#ec407a"/><rect x="15" y="45" width="12" height="25" rx="6" fill="#ffcc80"/><rect x="43" y="45" width="12" height="25" rx="6" fill="#ffcc80"/><rect x="22" y="70" width="10" height="20" fill="#424242"/><rect x="38" y="70" width="10" height="20" fill="#424242"/><rect x="25" y="50" width="20" height="20" rx="3" fill="#42a5f5"/></svg>
</div>
<div class="hero-content">
<h2>اختر الصف الدراسي للتعلم</h2>
<p>منهج اللغة العربية والتربية الدينية الإسلامية • الفصل الأول والثاني</p>
<p>شرح ومراجعة وبنوك أسئلة</p>
</div>
</section>

<h2 class="section-title">الدراسات - اختر الصف الآن للبدء</h2>

<div class="grades">
<div class="grade-card orange" onclick="openGrade(1)">
<div class="grade-icon">📖</div>
<h3>الصف الأول الثانوي</h3>
<p>اللغة العربية • التربية الدينية الإسلامية</p>
<div class="grade-tag">الفصل الأول والثاني - شرح ومراجعة • بنوك أسئلة</div>
<button class="grade-btn">اضغط للدخول</button>
</div>

<div class="grade-card blue" onclick="openGrade(2)">
<div class="grade-icon">📱</div>
<h3>الصف الثاني الثانوي</h3>
<p>اللغة العربية • التربية الدينية الإسلامية</p>
<div class="grade-tag">الفصل الأول والثاني - شرح ومراجعة • بنوك أسئلة</div>
<button class="grade-btn">اضغط للدخول</button>
</div>

<div class="grade-card yellow" onclick="openGrade(3)">
<div class="grade-icon">🎓</div>
<h3>الصف الثالث الثانوي</h3>
<p>اللغة العربية • التربية الدينية الإسلامية</p>
<div class="grade-tag">الفصل الأول والثاني - شرح ومراجعة • بنوك أسئلة</div>
<button class="grade-btn">اضغط للدخول</button>
</div>

<div class="stats">
<div class="stat-card"><div class="stat-icon">🌊</div><h4>طابع البحر الأحمر</h4></div>
<div class="stat-card"><div class="stat-icon">📚</div><h4>100+ درس تفاعلي</h4></div>
<div class="stat-card"><div class="stat-icon">❓</div><h4>2000+ سؤال تدريبي</h4></div>
<div class="stat-card"><div class="stat-icon">🏆</div><h4>اختبارات ومراجعات دورية</h4><p style="font-size:12px;margin-top:8px">🤖 جاهزون للتعلم!</p></div>
</div>

<footer class="footer">إعداد: مستر خالد المصري - معلم أول لغة عربية - مدرسة We البحر الأحمر</footer>
</div>

<div id="gradePage" class="page">
<button class="back-btn" onclick="goHome()">← رجوع للرئيسية</button>
<h2 id="gradeTitle" style="font-size:32px;margin-bottom:20px"></h2>
<div id="adminPanel" class="admin-panel">
<h3>➕ إضافة كتاب/درس جديد</h3>
<input type="text" id="bookTitle" placeholder="اسم الكتاب أو الدرس">
<select id="bookSubject"><option>لغة عربية</option><option>تربية دينية إسلامية</option></select>
<select id="bookSemester"><option>الفصل الأول</option><option>الفصل الثاني</option></select>
<textarea id="bookContent" placeholder="محتوى الدرس بالتشكيل الكامل..."></textarea>
<button class="ctrl-btn" onclick="addBook()">💾 حفظ الكتاب</button>
</div>
<div class="books-grid" id="booksGrid"></div>
</div>

<div id="lessonPage" class="page">
<button class="back-btn" onclick="backToGrade()">← رجوع للكتب</button>
<div class="lesson-view">
<h2 id="lessonTitle"></h2>
<div class="controls">
<button class="ctrl-btn" onclick="speakText()">🔊 قراءة صوتية</button>
<button class="ctrl-btn" onclick="changeFontSize(2)">🔍+ تكبير الخط</button>
<button class="ctrl-btn" onclick="changeFontSize(-2)">🔍- تصغير الخط</button>
<button class="ctrl-btn" onclick="toggleDark()">🌙 الوضع الليلي</button>
</div>
<div class="lesson-text" id="lessonText"></div>
</div>

<script>
let currentGrade=1,currentBooks=[],fontSize=20,isDark=false,adminClicks=0;
let deferredPrompt;

// بيانات الكتب من الملفات اللي رفعتها
const allBooks={
1:[
{title:"التربية الدينية الإسلامية - الوحدة الأولى",subject:"تربية دينية إسلامية",semester:"الفصل الأول",icon:"🕌",content:`<h3>الدرس الأول: الإيمانُ باللهِ الواحدِ الأَحَدِ</h3>
<p><b>الأهداف:</b><br>
• أنْ يَعْرِفَ أُصُولَ العَقِيدَةِ الإسلامِيَّةِ.<br>
• أنْ يَتَمَسَّكَ بِوَحْدَانِيَّةِ اللهِ مِن خِلالِ الآياتِ الشَّرْعِيَّةِ.<br>
• أنْ يَسْتَخْدِمَ الأدِلَّةَ العَقْلِيَّةَ والنَّقْلِيَّةَ في إقْناعِ المُنْكِرِينَ لِوَحْدَانِيَّةِ اللهِ.</p>
<p><b>الأدِلَّةُ الكَوْنِيَّةُ على وُجُودِ اللهِ:</b><br>
الكَوْنُ يَدُلُّ على وُجُودِ خالِقِهِ، وكُلَّما تَأَمَّلَ الإنْسانُ الكَوْنَ زادَ يَقِينُهُ باللهِ.<br>
مِنَ الأمْثِلَةِ: البَعْرَةُ تَدُلُّ على البَعِيرِ، وآثارُ الأقْدَامِ تَدُلُّ على المَسِيرِ.</p>
<p><b>مَعْنَى الوَحْدَانِيَّةِ:</b><br>
الوَحْدَانِيَّةُ: أنَّ اللهَ واحِدٌ لا شَرِيكَ لَهُ، فَرْدٌ صَمَدٌ.<br>
قالَ تَعالى: ﴿وَلَمْ يَكُن لَّهُ كُفُوًا أَحَدٌ﴾، أي لَمْ يَكُنْ لَهُ نَظِيرٌ ولا مَثِيلٌ.</p>`},
{title:"التربية الدينية - الوحدة الثانية: الزوجة المجادلة",subject:"تربية دينية إسلامية",semester:"الفصل الأول",icon:"🕌",content:`<h3>سورةُ المُجادَلَةِ</h3>
<p><b>قِصَّةُ السُّورَةِ:</b><br>
نَزَلَتِ السُّورَةُ في خَوْلَةَ بِنْتِ ثَعْلَبَةَ رَضِيَ اللهُ عَنْها، حِينَ ظاهَرَ مِنْها زَوْجُها أَوْسُ بنُ الصَّامِتِ رَضِيَ اللهُ عَنْهُ.</p>
<p><b>الظِّهَارُ:</b><br>
أنْ يُشَبِّهَ الرَّجُلُ زَوْجَتَهُ بِأُمِّهِ، فَيَقُولَ لَها: «أَنْتِ عَلَيَّ كَظَهْرِ أُمِّي».<br>
الظِّهَارُ مُنْكَرٌ مِنَ القَوْلِ وزُورٌ، وهُوَ مُحَرَّمٌ في الإسلامِ.</p>
<p><b>كَفَّارَةُ الظِّهَارِ:</b><br>
تَحْرِيرُ رَقَبَةٍ، فإنْ لَمْ يَجِدْ فَصِيامُ شَهْرَيْنِ مُتَتابِعَيْنِ، فإنْ لَمْ يَسْتَطِعْ فَإطْعامُ سِتِّينَ مِسْكِينًا.</p>`}
],
2:[
{title:"اللغة العربية - للصف الثاني الثانوي الفني",subject:"لغة عربية",semester:"الفصل الأول",icon:"📗",content:`<h3>القِراءَةُ</h3>
<p><b>الموضوعات:</b><br>
1. هَلْ لَدَيْكَ هَدَفٌ في الحَياةِ؟<br>
2. قِيمَةُ العَمَلِ<br>
3. أهَمِّيَّةُ الرِّياضَةِ</p>
<h3>الأدَبُ والنُّصُوصُ</h3>
<p>العَصْرُ العَبَّاسِيُّ والأَنْدَلُسِيُّ</p>
<h3>البَلاغَةُ</h3>
<p>عِلمُ المَعانِي - الخَبَرُ والإِنْشاءُ</p>
<h3>النَّحْوُ</h3>
<p>المَفْعُولُ المُطْلَقُ - المَفْعُولُ لأَجْلِهِ - الحالُ</p>
<h3>الإمْلاءُ</h3>
<p>عَلاماتُ التَّرْقِيمِ - الألِفُ اللَّيِّنَةُ</p>`}
],
3:[]
};

window.addEventListener('beforeinstallprompt',(e)=>{e.preventDefault();deferredPrompt=e;document.getElementById('installBtn').style.display='block'});
document.getElementById('installBtn').onclick=()=>{if(deferredPrompt){deferredPrompt.prompt()}};

document.getElementById('logoClick').onclick=()=>{adminClicks++;if(adminClicks>=5){document.getElementById('adminPanel').classList.add('active');alert('تم تفعيل وضع المدير')}};

function openGrade(grade){
currentGrade=grade;
document.getElementById('mainPage').style.display='none';
document.getElementById('gradePage').classList.add('active');
document.getElementById('gradeTitle').textContent=`الصف ${grade===1?'الأول':grade===2?'الثاني':'الثالث'} الثانوي`;
loadBooks();
}

function goHome(){
document.getElementById('gradePage').classList.remove('active');
document.getElementById('mainPage').style.display='block';
}

function loadBooks(){
const grid=document.getElementById('booksGrid');
const books=allBooks[currentGrade]||[];
if(books.length===0){
grid.innerHTML='<p style="text-align:center;color:#546e7a;font-size:18px">لا توجد كتب مضافة بعد. فعل وضع المدير لإضافة محتوى.</p>';
return;
}
grid.innerHTML=books.map((book,i)=>`
<div class="book-card" onclick="openLesson(${i})">
<div class="book-icon">${book.icon}</div>
<h4>${book.title}</h4>
<p>${book.subject} • ${book.semester}</p>
</div>`).join('');
}

function openLesson(idx){
const book=allBooks[currentGrade][idx];
document.getElementById('gradePage').classList.remove('active');
document.getElementById('lessonPage').classList.add('active');
document.getElementById('lessonTitle').textContent=book.title;
document.getElementById('lessonText').innerHTML=book.content;
}

function backToGrade(){
document.getElementById('lessonPage').classList.remove('active');
document.getElementById('gradePage').classList.add('active');
}

function speakText(){
const text=document.getElementById('lessonText').innerText;
const utterance=new SpeechSynthesisUtterance(text);
utterance.lang='ar-SA';
utterance.rate=0.9;
speechSynthesis.speak(utterance);
}

function changeFontSize(delta){
fontSize+=delta;
document.getElementById('lessonText').style.fontSize=fontSize+'px';
}

function toggleDark(){
isDark=!isDark;
document.querySelector('.lesson-view').style.background=isDark?'#263238':'#fff';
document.querySelector('.lesson-view').style.color=isDark?'#fff':'#263238';
}

function addBook(){
const title=document.getElementById('bookTitle').value;
const subject=document.getElementById('bookSubject').value;
const semester=document.getElementById('bookSemester').value;
const content=document.getElementById('bookContent').value;
if(!title||!content){alert('اكتب العنوان والمحتوى');return}
if(!allBooks[currentGrade])allBooks[currentGrade]=[];
allBooks[currentGrade].push({title,subject,semester,content,icon:subject.includes('دينية')?'🕌':'📗'});
loadBooks();
alert('تم إضافة الكتاب بنجاح');
document.getElementById('bookTitle').value='';
document.getElementById('bookContent').value='';
}
</script>
</body>
</html>
منصة تعليمية
