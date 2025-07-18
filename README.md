<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="stely.css">
    <title>Document</title>
</head>
<body>

    <header class="header">
        <h1 class="Logo">Logo</h1>

        <div class="h-inner">
            
            <a href="#" class="link">Content</a>
            <a href="#" class="link">About Us</a>
            <a href="#" class="link">Reviews</a>
            <a href="#" class="link">Your project</a>
            
        </div>
        
        

        <a href="#" class="h-btn">Menu</a>

        
    </header>
        <div class="language-switcher">
            <button onclick="setLanguage('ru')">RU</button> |
            <button onclick="setLanguage('en')">EN</button>
        </div>

    <section class="sub-main">
        <h1 class="sm-title" data-key="main-title">Мы строим дома, которые служат веками</h1>
        <p class="sm-text" data-key="main-subtitle">Абсолютно новый подход к строительству от европейских инженеров</p>
    </section>

    <main class="main">

        

        <div class="cards-container">
            <div class="div1">
                <div class="card1"></div>
                <p class="text">This project was developed by our professional<br> architects taking into account modern SNiPs and GOSTs.</p>
                <a href="#" class="gam">Look</a>
            </div>

            <div class="div2">
                <div class="card2"></div>
                <p class="text">  During construction, bitumen shingles (soft tiles) and metal tiles are <br>interchangeable and do not require additional changes in the project.</p>
                <a href="#" class="gam">Look</a>
            </div>

            <div class="div3">
                <div class="card3"></div>
                <p class="text">Package of drawings and technical data <br>  AS-2585 is a working construction document</p>
                <a href="#" class="gam">Look</a>
            </div>
        </div>
        <div class="banner">
            🔥 Специальное предложение! Только сегодня -50%! <br>

            <button>Узнать больше</button>
        </div>

    <script>
    const translations = {
     ru: {
        "main-title": "Мы строим дома, которые служат веками",
        "main-subtitle": "Абсолютно новый подход к строительству от европейских инженеров",
        "btn-look": "Смотреть",
     },
     en: {
        "main-title": "We build houses that last",
        "main-subtitle": "A revolutionary new approach to housing by European engineers",
        "btn-look": "Look",
    }
};

function setLanguage(lang) {
    document.querySelectorAll("[data-key]").forEach(el => {
    const key = el.getAttribute("data-key");
    el.textContent = translations[lang][key] || el.textContent;
  });
}
</script>
        
    </main>

    <title>Рекламный баннер</title>

    <section>
        We have been building reliably since 2008. Houses, offices, warehouses and turnkey commercial real estate<br>

        Адрес: г. Москва, ул. Строителей, 15,

        Телефон: +7 (495) 123-45-67. <br>

        Email: info@stroymaster.ru, 

        Режим работы: Пн–Пт, 9:00–18:00. <br>
    </section>
</body>
</html>


@import url('https://fonts.googleapis.com/css2?family=Lato:ital,wght@0,100;0,300;0,400;0,700;0,900;1,100;1,300;1,400;1,700;1,900&family=Manufacturing+Consent&family=Montserrat:ital,wght@0,100..900;1,100..900&family=Open+Sans:ital,wght@0,300..800;1,300..800&family=Playfair:ital,opsz,wght@0,5..1200,300..900;1,5..1200,300..900&family=Roboto:ital,wght@0,100..900;1,100..900&display=swap');

*{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    font-family: "Montserrat", sans-serif;
    background: url(ChatGPT\ Image\ 8\ июл.\ 2025\ г.\,\ 19_56_56.png) center center no-repeat;
    background-size: cover;
    
}

.sub-main {
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
}

.sm-title {
    font-size: 5em;
    color: white;
}

.sm-text {
    font-size: 1.5em;
    color: white;
}

.main {
    height: 100vh;
    font-size: 2em;
}

.header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 2em;
    margin: 10px;
}

.language-switcher {
  display: flex;
  gap: 10px;
  align-items: center;
}

.language-switcher button {
  background: transparent;
  color: white;
  border: 1px solid white;
  padding: 5px 10px;
  cursor: pointer;
  transition: 0.3s ease;
}

.language-switcher button:hover {
  background-color: white;
  color: black;
}

a {
    text-decoration: none;
    color: rgb(255, 255, 255);
    font-size: 20px;
}

.h-inner {
    display: flex;
    gap: 80px;
}

.Logo {
    display: flex;
    color: rgb(255, 255, 255);
}

.h-btn {
    border: 2px solid rgb(255, 255, 255);
    border-radius: 8px;
    padding: 10px 25px;
    background-color: transparent;
    color: white;
    cursor: pointer;
    transition: all 0.3s ease;
}

.h-btn:hover {
    background-color: white;
    color: black;
    transform: scale(1.05); 
}

.cards-container {
    display: flex;
    gap: 50px;
    justify-content: center;
    align-items: flex-start;
    padding: 20px; 
    flex-wrap: wrap;
}

.div1, .div2, .div3 {
    width: 530px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    gap: 20px;
} 

.card1 {
    width: 530px;
    height: 330px;
    background-color: rgb(80, 80, 80);
    border: 1px solid #ffffff;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    display: flex;
    
    font-size: 18px;
}

.card2 {
    width: 530px;
    height: 330px;
    background-color: rgb(80, 80, 80);
    border: 1px solid #ffffff;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    display: flex;
    
    font-size: 18px;
}

.card3 {
    width: 530px;
    height: 330px;
    background-color: rgb(80, 80, 80);
    border: 1px solid #ffffff;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    display: flex;
    
    font-size: 18px;
}

.text {
    color: white;
    font-size: 18px;
}

section {
    padding: 20px;
    font-size: 18px;
    line-height: 1.6;
    text-align: center;
}

.gam {
    border: 2px solid rgb(255, 255, 255);
    border-radius: 8px;
    padding: 5px 15px;
    background-color: transparent;
    color: white;
    cursor: pointer;
    transition: all 0.5s ease;
}

.gam:hover {
    background-color: white;
    color: black;
    transform: scale(1.05); 
}

.card3 {
  background-image: url(as-2585.webp);
  background-size: cover;
  transition: 0.5s ease;
}

.card3:hover {
  background-image: url('as-2585_1.webp');
}

.card2 {
  background-image: url(as-2584.webp);
  background-size: cover;
  transition: 0.5s ease;
}

.card2:hover {
  background-image: url(as-2584_1.webp)
}

.card1 {
  background-image: url(as-2607.webp);
  background-size: cover;
  transition: 0.5s ease;
}

.card1:hover {
  background-image: url('as-2607_1.webp');
}

.banner {
    background: linear-gradient(135deg, #ff9800, #f44336);
    color: white;
    padding: 20px 40px;
    text-align: center;
    font-family: sans-serif;
    font-size: 24px;
    border-radius: 12px;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.3);
    max-width: 600px;
    margin: 40px auto;
    position: relative;
}

.banner button {
    margin-top: 15px;
    padding: 10px 20px;
    background-color: white;
    color: #f44336;
    border: none;
    border-radius: 8px;
    font-size: 16px;
    cursor: pointer;
    transition: 0.3s ease;
}

.banner button:hover {
    background-color: #ffe3e3;
}
