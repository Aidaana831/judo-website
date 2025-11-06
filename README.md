<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Дзюдо: Путь гармонии и силы</title>
    <style>
        /* Общие стили */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #f8f9fa;
            color: #333;
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Шапка */
        header {
            background: linear-gradient(to right, #1a1a1a, #2d2d2d);
            padding: 20px 0;
            border-bottom: 4px solid #c41e3a;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 28px;
            font-weight: bold;
            color: #fff;
        }
        
        .logo span {
            color: #c41e3a;
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 25px;
        }
        
        nav ul li a {
            color: #fff;
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s;
            padding: 8px 15px;
            border-radius: 5px;
        }
        
        nav ul li a:hover, nav ul li a.active {
            color: #c41e3a;
            background-color: rgba(255, 255, 255, 0.1);
        }
        
        /* Основной контент */
        main {
            padding: 40px 0;
            min-height: calc(100vh - 160px);
        }
        
        .page {
            display: none;
            animation: fadeIn 0.5s ease-in;
        }
        
        .page.active {
            display: block;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        h1 {
            font-size: 36px;
            margin-bottom: 20px;
            color: #c41e3a;
            text-align: center;
        }
        
        h2 {
            font-size: 28px;
            margin: 30px 0 15px;
            color: #333;
            border-bottom: 2px solid #c41e3a;
            padding-bottom: 10px;
        }
        
        h3 {
            font-size: 22px;
            margin: 20px 0 10px;
            color: #555;
        }
        
        p {
            margin-bottom: 15px;
            text-align: justify;
        }
        
        .hero {
            text-align: center;
            padding: 60px 0;
            background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="100" height="100" viewBox="0 0 100 100"><rect width="100" height="100" fill="%232d2d2d"/><path d="M30,30 L70,70 M70,30 L30,70" stroke="%23c41e3a" stroke-width="8"/></svg>');
            background-size: cover;
            color: white;
            border-radius: 10px;
            margin-bottom: 40px;
        }
        
        .hero h1 {
            color: white;
            font-size: 42px;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
        }
        
        .hero p {
            max-width: 800px;
            margin: 0 auto 20px;
            font-size: 18px;
        }
        
        .btn {
            display: inline-block;
            background: linear-gradient(to right, #c41e3a, #e63946);
            color: white;
            padding: 12px 25px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: bold;
            transition: transform 0.3s, box-shadow 0.3s;
            margin-top: 10px;
            border: none;
            cursor: pointer;
        }
        
        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(196, 30, 58, 0.4);
        }
        
        /* Карточки */
        .cards {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 25px;
            margin-top: 30px;
        }
        
        .card {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            transition: transform 0.3s, box-shadow 0.3s;
            border: 1px solid #ddd;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }
        
        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.15);
        }
        
        .card-img {
            height: 180px;
            background-color: #2d2d2d;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 60px;
            color: white;
        }
        
        .card-content {
            padding: 20px;
        }
        
        .card h3 {
            font-size: 22px;
            margin-bottom: 10px;
            color: #c41e3a;
        }
        
        /* Таблица */
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
            background-color: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }
        
        th, td {
            padding: 12px 15px;
            text-align: left;
            border-bottom: 1px solid #ddd;
        }
        
        th {
            background-color: #2d2d2d;
            color: white;
        }
        
        tr:hover {
            background-color: #f9f9f9;
        }
        
        /* Подвал */
        footer {
            background: linear-gradient(to right, #1a1a1a, #2d2d2d);
            padding: 30px 0;
            border-top: 4px solid #c41e3a;
            text-align: center;
            color: white;
        }
        
        .footer-content {
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        
        .social-links {
            display: flex;
            margin: 20px 0;
        }
        
        .social-links a {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background-color: #444;
            border-radius: 50%;
            margin: 0 10px;
            color: white;
            text-decoration: none;
            transition: background-color 0.3s;
        }
        
        .social-links a:hover {
            background-color: #c41e3a;
        }
        
        .copyright {
            margin-top: 20px;
            color: #ccc;
            font-size: 14px;
        }
        
        /* Адаптивность */
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
            }
            
            nav ul {
                margin-top: 15px;
                flex-wrap: wrap;
                justify-content: center;
            }
            
            nav ul li {
                margin: 5px 10px;
            }
            
            h1 {
                font-size: 30px;
            }
            
            .hero h1 {
                font-size: 34px;
            }
        }
        
        /* Специфические стили для дзюдо */
        .quote {
            font-style: italic;
            background-color: #f9f9f9;
            border-left: 4px solid #c41e3a;
            padding: 15px;
            margin: 20px 0;
            border-radius: 0 8px 8px 0;
        }
        
        .technique-list {
            list-style-type: none;
            padding-left: 0;
        }
        
        .technique-list li {
            padding: 8px 0;
            border-bottom: 1px solid #eee;
        }
        
        .technique-list li:before {
            content: "•";
            color: #c41e3a;
            font-weight: bold;
            display: inline-block;
            width: 1em;
            margin-left: -1em;
        }
        
        .belt-system {
            display: flex;
            justify-content: space-between;
            margin: 30px 0;
            flex-wrap: wrap;
        }
        
        .belt {
            text-align: center;
            margin: 10px;
            flex: 1;
            min-width: 100px;
        }
        
        .belt-color {
            height: 25px;
            margin-bottom: 10px;
            border-radius: 5px;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }
        
        .white { background-color: white; border: 1px solid #ddd; }
        .yellow { background-color: #ffeb3b; }
        .orange { background-color: #ff9800; }
        .green { background-color: #4caf50; }
        .blue { background-color: #2196f3; }
        .brown { background-color: #795548; }
        .black { background-color: #000; color: white; }
        
        .philosophy-principles {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            margin: 30px 0;
        }
        
        .principle {
            flex: 1;
            min-width: 300px;
            background: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }
        
        .principle h3 {
            color: #c41e3a;
            border-bottom: 1px solid #eee;
            padding-bottom: 10px;
        }
        
        .personal-story {
            background: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
            margin: 20px 0;
        }
        
        .personal-story h3 {
            color: #c41e3a;
        }
        
        .content-img {
            width: 100%;
            height: 200px;
            background-color: #eee;
            border-radius: 8px;
            margin: 15px 0;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 40px;
            color: #777;
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <div class="header-content">
                <div class="logo">Дзюдо<span>Путь</span></div>
                <nav>
                    <ul>
                        <li><a href="#" class="nav-link active" data-page="home">Главная</a></li>
                        <li><a href="#" class="nav-link" data-page="philosophy">Философия</a></li>
                        <li><a href="#" class="nav-link" data-page="techniques">Техники</a></li>
                        <li><a href="#" class="nav-link" data-page="personal">Мой путь</a></li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>
    
    <main class="container">
        <!-- Главная страница -->
        <section id="home" class="page active">
            <div class="hero">
                <h1>Дзюдо: Искусство мягкости и путь самосовершенствования</h1>
                <p>Откройте для себя мир дзюдо - боевого искусства, которое учит не только самообороне, но и философии жизни, основанной на взаимном уважении и максимальной эффективности.</p>
                <a href="#" class="btn nav-link" data-page="philosophy">Узнать о философии</a>
            </div>
            
            <h2>Что такое дзюдо?</h2>
            <p>Дзюдо — это японское боевое искусство, созданное Дзигоро Кано в 1882 году. Название переводится как "мягкий путь" или "гибкий путь". В отличие от многих других боевых искусств, дзюдо делает акцент не на силе, а на технике, гибкости и использовании силы противника против него самого.</p>
            
            <p>Лично для меня дзюдо — это не просто спорт или боевое искусство. Это философия жизни, которая учит адаптироваться к обстоятельствам, находить оптимальные решения в сложных ситуациях и постоянно работать над собой. Когда я начала заниматься дзюдо в 9 лет, я даже не представляла, насколько сильно это повлияет на мой характер и мировоззрение.</p>
            
            <h2>Почему я выбрал дзюдо?</h2>
            <p>Мой путь в дзюдо начался довольно необычно. Однажды мой папа отвел меня на тренировку, и хотя сначала я сомневалась, это решение изменило мою жизнь. Дзюдо научило меня не только защищать себя, но и уверенно идти к своим целям, уважать других и никогда не сдаваться.</p>
            
            <div class="cards">
                <div class="card">
                    <div class="card-img">🥋</div>
                    <div class="card-content">
                        <h3>Физическое развитие</h3>
                        <p>Дзюдо развивает силу, гибкость, координацию и выносливость. Регулярные тренировки укрепляют все группы мышц.</p>
                    </div>
                </div>
                <div class="card">
                    <div class="card-img">🧠</div>
                    <div class="card-content">
                        <h3>Психическое развитие</h3>
                        <p>Тренировки развивают дисциплину, концентрацию, уверенность в себе и умение принимать быстрые решения.</p>
                    </div>
                </div>
                <div class="card">
                    <div class="card-img">🤝</div>
                    <div class="card-content">
                        <h3>Социальные аспекты</h3>
                        <p>Дзюдо учит уважению, сотрудничеству и взаимопомощи. В дзюдо создается особая атмосфера товарищества.</p>
                    </div>
                </div>
            </div>
        </section>
        
        <!-- Философия дзюдо -->
        <section id="philosophy" class="page">
            <h1>Философия дзюдо</h1>
            <p>Дзюдо — это не просто спорт или боевое искусство. Это целостная система воспитания личности, основанная на глубоких философских принципах, которые применимы не только на татами, но и в повседневной жизни.</p>
            
            <div class="quote">
                "Дзюдо — это путь к наиболее эффективному использованию физической и духовной энергии. Посредством тренировок в нападении и защите вы развиваете свое тело и душу, и это воплощается в сущность вашего бытия. Таким образом, вы совершенствуете себя и вносите вклад в развитие общества. Это конечная цель практики дзюдо." — Дзигоро Кано
            </div>
            
            <h2>Два основных принципа дзюдо</h2>
            
            <div class="philosophy-principles">
                <div class="principle">
                    <h3>Сэйрёку дзэнъё</h3>
                    <p>Наиболее эффективное использование духовной и физической энергии. Этот принцип учит нас, что в любой ситуации нужно искать самый эффективный путь достижения цели с минимальными затратами энергии.</p>
                    <p>В дзюдо это проявляется в технике — вместо того, чтобы противостоять силе противника напрямую, мы используем его движение и силу против него самого.</p>
                    <p>В жизни этот принцип помогает мне находить оптимальные решения проблем, не тратя силы на бесполезное сопротивление обстоятельствам, а адаптируясь к ним и используя их в своих интересах.</p>
                </div>
                
                <div class="principle">
                    <h3>Дзита кёэй</h3>
                    <p>Взаимное благоденствие для себя и других. Дзигоро Кано считал, что практика дзюдо должна приносить пользу не только самому практикующему, но и обществу в целом.</p>
                    <p>Тренируясь вместе, мы помогаем друг другу совершенствоваться. Партнер не является врагом — он помогает нам расти, а мы помогаем расти ему.</p>
                    <p>Этот принцип я стараюсь применять в повседневной жизни: сотрудничество и взаимопомощь часто приносят больше пользы, чем конкуренция и противостояние.</p>
                </div>
            </div>
            
            <h2>Воспитание характера через дзюдо</h2>
            <p>Дзюдо — это мощный инструмент формирования характера. Регулярные тренировки развивают не только физические качества, но и важные личностные характеристики, которые остаются с человеком на всю жизнь.</p>
            
            <ul class="technique-list">
                <li><strong>Дисциплина</strong> — регулярные тренировки требуют самоконтроля и организованности. Я помню, как сложно было сначала заставлять себя идти на тренировки после тяжелого учебного дня, но со временем это вошло в привычку и стало частью моей жизни.</li>
                <li><strong>Уважение</strong> — к тренеру, партнерам, противникам и самому себе. В дзюдо уважение проявляется не только в словах, но и в действиях — в аккуратном обращении с формой, в правильном выполнении поклонов, в бережном отношении к партнеру во время отработки приемов.</li>
                <li><strong>Настойчивость</strong> — падения и неудачи являются неотъемлемой частью пути к мастерству. Каждый раз, когда ты падаешь, ты должен подняться и попробовать снова. Эта простая истина стала для меня метафорой жизни.</li>
                <li><strong>Смирение</strong> — даже самый опытный дзюдоист всегда может чему-то научиться. Я видела, как обладатели черных поясов с уважением относились к советам менее опытных товарищей, если те делились с ценноой информацией.</li>
                <li><strong>Ответственность</strong> — за свою безопасность и безопасность партнера. Когда ты выполняешь бросок, ты отвечаешь не только за себя, но и за того, кого бросаешь. Это учит думать о последствиях своих действий.</li>
            </ul>
        </section>
        
        <!-- Техники дзюдо -->
        <section id="techniques" class="page">
            <h1>Техники дзюдо</h1>
            <p>Технический арсенал дзюдо богат и разнообразен. Он включает в себя броски, удержания, болевые приемы и удушения. Все техники делятся на несколько основных групп, каждая из которых имеет свою специфику и область применения.</p>
            
            <h2>Нагэ-вадза (техника бросков)</h2>
            <p>Броски в дзюдо — это основа основ. Они делятся на несколько групп в зависимости от того, какая часть тела используется как главный инструмент броска.</p>
            
            <table>
                <thead>
                    <tr>
                        <th>Группа бросков</th>
                        <th>Принцип</th>
                        <th>Примеры техник</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>Тэ-вадза (броски руками)</td>
                        <td>Использование в основном рук для выполнения броска</td>
                        <td>Сэойнагэ, Тайотоси, Катагурума</td>
                    </tr>
                    <tr>
                        <td>Коси-вадза (броски бедром)</td>
                        <td>Использование бедер как точки опоры</td>
                        <td>Огоси, Цурикомигоси, Ханегоси</td>
                    </tr>
                    <tr>
                        <td>Аси-вадза (броски ногами)</td>
                        <td>Подсечки и зацепы ногами</td>
                        <td>Осотогари, Оучигари, Косотогари</td>
                    </tr>
                    <tr>
                        <td>Масутэми-вадза (броски с падением)</td>
                        <td>Броски с падением атакующего</td>
                        <td>Томоэнагэ, Сумигаэси, Хикикомигаэси</td>
                    </tr>
                </tbody>
            </table>
            
            <h2>Катамэ-вадза (техника обездвиживания)</h2>
            <p>После броска дзюдоист переходит к технике обездвиживания, которая включает удержания, удушающие и болевые приемы.</p>
            
            <ul class="technique-list">
                <li><strong>Осаэкоми-вадза</strong> — удержания (Кэсагатамэ, Камисихогатамэ, Ёкосифогатамэ)</li>
                <li><strong>Симэ-вадза</strong> — удушающие приемы (Намидзюдзидзимэ, Катадзюдзидзимэ, Хадкадзимэ)</li>
                <li><strong>Кансэцу-вадза</strong> — болевые приемы на суставы (Дзюдзигатамэ, Удэгарамэ, Асигатамэ)</li>
            </ul>
            
            <h2>Система поясов в дзюдо</h2>
            <p>В дзюдо существует система поясов (кю и даны), отражающая уровень мастерства. Каждый цвет пояса символизирует определенный этап развития дзюдоиста.</p>
            
            <div class="belt-system">
                <div class="belt">
                    <div class="belt-color white"></div>
                    <div>6 кю</div>
                </div>
                <div class="belt">
                    <div class="belt-color yellow"></div>
                    <div>5 кю</div>
                </div>
                <div class="belt">
                    <div class="belt-color orange"></div>
                    <div>4 кю</div>
                </div>
                <div class="belt">
                    <div class="belt-color green"></div>
                    <div>3 кю</div>
                </div>
                <div class="belt">
                    <div class="belt-color blue"></div>
                    <div>2 кю</div>
                </div>
                <div class="belt">
                    <div class="belt-color brown"></div>
                    <div>1 кю</div>
                </div>
                <div class="belt">
                    <div class="belt-color black"></div>
                    <div>1-10 дан</div>
                </div>
            </div>
            
            <p>Когда я получил свой первый пояс (белый), я думала, что это просто формальность. Но со временем я поняла, что каждый новый цвет — это не просто полоска ткани, а символ пройденного пути, преодоленных трудностей и новых обязательств.</p>
            
            <h2>Мои любимые техники</h2>
            <p>За годы тренировок у меня сформировались свои предпочтения в технике. Особенно мне нравятся броски из группы аси-вадза, такие как о-сото-гари и коучи-гари. Эти техники требуют хорошего чувства времени и баланса, но когда они выполняются правильно, выглядят очень элегантно и эффективно.</p>
            
            <p>Также я ценю технику удержаний, особенно кэса-гатамэ. Эта техника учит не только контролировать противника, но и сохранять спокойствие и концентрацию в стрессовой ситуации.</p>
        </section>
        
        <!-- Мой путь в дзюдо -->
        <section id="personal" class="page">
            <h1>Мой путь в дзюдо</h1>
            <p>Мое знакомство с дзюдо началось в детстве, и с тех пор это искусство стало неотъемлемой частью моей жизни. На этой странице я хочу поделиться своим личным опытом и тем, как дзюдо повлияло на мою жизнь.</p>
            
            <div class="personal-story">
                <h3>Начало пути</h3>
                <p>Я начал заниматься дзюдо в 9 лет. Помню, как сначала меня отвел мой папа на отборочные соревнования после того, как ему об этом сообщил его друг. Поначалу меня привлекла зрелищность бросков, но со временем я поняла, что дзюдо — это нечто гораздо большее, чем просто спорт. Мой первый тренер часто повторял: "Дзюдо начинается с поклона и заканчивается поклоном". Эти слова я понял не сразу, но со временем осознал их глубокий смысл.</p>
                <div class="content-img">🥋 Первая тренировка</div>
            </div>
            
            <div class="personal-story">
                <h3>Первые трудности</h3>
                <p>Первые месяцы тренировок были непростыми. Постоянные падения, синяки и чувство неловкости при выполнении приемов заставляли меня сомневаться в своем выборе. Но именно в этот период я научилась самому важному — умению падать и подниматься.</p>
                <p>Мой тренер говорил: "Тот, кто научился правильно падать, уже наполовину победил". Со временем я поняла, что это относится не только к дзюдо, но и к жизни в целом.</p>
                <div class="content-img">🔄 Падения и подъемы</div>
            </div>
            
            <div class="personal-story">
                <h3>Первый успех</h3>
                <p>Помню свой первый турнир. Я была очень нервной и сильно переживала, что почти не спала. Но когда я вышла на татами, все волнение куда-то исчезло. В тот день я выиграла свою первую медаль и подарок ввиде шоколадки "Аленка". Это была не самая ценная награда в моей жизни, но одна из самых значимых.</p>
                <p>Этот опыт научил меня, что подготовка и уверенность в себе часто важнее природного таланта.</p>
                <div class="content-img">🏆 Первая медаль</div>
            </div>
            
            <div class="personal-story">
                <h3>Дзюдо в повседневной жизни</h3>
                <p>Принципы дзюдо я применяю не только на татами, но и в повседневной жизни. Например, принцип "мягкость побеждает силу" помогает мне в решении конфликтов — вместо того чтобы идти на прямое противостояние, я стараюсь найти компромисс, который устроит всех.</p>
                <p>Принцип максимальной эффективности помогает в работе — я научилась определять, какие задачи действительно важны, и сосредотачиваться на них, не тратя силы на второстепенное.</p>
                <p>Но самое главное, чему научило меня дзюдо — это умение "падать" и "подниматься". В жизни, как и на татами, бывают неудачи и поражения. Дзюдо научило меня принимать их не как трагедию, а как возможность для роста, анализа ошибок и движения вперед.</p>
                <div class="content-img">💡 Применение в жизни</div>
            </div>
            
            <div class="personal-story">
                <h3>Советы начинающим</h3>
                <p>Если вы только начинаете свой путь в дзюдо, вот несколько советов из моего опыта:</p>
                <ul class="technique-list">
                    <li>Не стремитесь сразу к сложным броскам — освойте сначала базовую технику и укэми</li>
                    <li>Будьте терпеливы — прогресс в дзюдо требует времени и регулярных тренировок</li>
                    <li>Не бойтесь проигрывать — каждое поражение это ценный урок</li>
                    <li>Уважайте своих партнеров — без них ваш прогресс был бы невозможен</li>
                    <li>Наслаждайтесь процессом — дзюдо это не только результат, но и сам путь</li>
                </ul>
            </div>
            
            <div class="quote">
                "Самое главное в дзюдо — не победа, а совершенство характера. Дзюдо не для того, чтобы стать сильнее других, а для того, чтобы стать лучше себя вчерашнего."
            </div>
            
            <p>Дзюдо — это искусство, которое сопровождало меня много лет до серьезной травмы, но уверена, что оно будет со мной всю жизнь ментально. Оно научило меня не только защищать себя, но и понимать других, адаптироваться к изменениям и постоянно стремиться к самосовершенствованию.</p>
        </section>
    </main>
    
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="logo">Дзюдо<span>Путь</span></div>
                <p>Искусство мягкости и путь самосовершенствования</p>
                <div class="social-links">
                    <a href="#">FB</a>
                    <a href="#">IG</a>
                    <a href="#">YT</a>
                    <a href="#">TW</a>
                </div>
                <div class="copyright">
                    &copy; 2023 ДзюдоПуть. Сайт создан с интересом к искусству дзюдо.
                </div>
            </div>
        </div>
    </footer>

    <script>
        // JavaScript для навигации между страницами
        document.addEventListener('DOMContentLoaded', function() {
            const navLinks = document.querySelectorAll('.nav-link');
            const pages = document.querySelectorAll('.page');
            
            // Функция для активации страницы
            function activatePage(pageId) {
                // Скрываем все страницы
                pages.forEach(page => {
                    page.classList.remove('active');
                });
                
                // Убираем активный класс со всех ссылок
                navLinks.forEach(link => {
                    link.classList.remove('active');
                });
                
                // Показываем выбранную страницу
                document.getElementById(pageId).classList.add('active');
                
                // Добавляем активный класс к текущей ссылке
                document.querySelector(`.nav-link[data-page="${pageId}"]`).classList.add('active');
                
                // Прокручиваем к началу страницы
                window.scrollTo(0, 0);
            }
            
            // Обработчики для навигационных ссылок
            navLinks.forEach(link => {
                link.addEventListener('click', function(e) {
                    e.preventDefault();
                    const pageId = this.getAttribute('data-page');
                    activatePage(pageId);
                });
            });
            
            // Обработка загрузки страницы с хэшем в URL
            window.addEventListener('load', function() {
                const hash = window.location.hash.substring(1);
                if (hash && document.getElementById(hash)) {
                    activatePage(hash);
                }
            });
        });
    </script>
</body>
</html>
