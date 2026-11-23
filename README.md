<!doctype html>
<html lang="ru">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="theme-color" content="#11121a">
<title>OMNIX CLAN — Правила</title>

<style>
:root {
  color-scheme: dark;
  --bg: #101119;
  --text: #f2f1f7;
  --muted: #aaaaba;
  --accent: #c8c7d9;
  --line: rgba(225,226,241,.16);
}

* {
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  margin: 0;
  min-height: 100vh;
  background:
    radial-gradient(ellipse at 50% -15%, #44445c 0, transparent 48%),
    radial-gradient(ellipse at 100% 70%, #29283d 0, transparent 35%),
    var(--bg);
  color: var(--text);
  font-family: Inter, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
  line-height: 1.65;
}

body:before {
  content: "";
  position: fixed;
  inset: 0;
  pointer-events: none;
  opacity: .12;
  background-image:
    linear-gradient(120deg, transparent 48%, #a9a8c0 49%, transparent 50%),
    linear-gradient(60deg, transparent 48%, #a9a8c0 49%, transparent 50%);
  background-size: 180px 260px;
}

.wrap {
  width: min(900px, calc(100% - 32px));
  margin: auto;
  padding: 58px 0 36px;
  position: relative;
}

.hero {
  text-align: center;
  padding: 30px 18px 38px;
}

.sigil {
  font-size: 25px;
  letter-spacing: 13px;
  color: var(--accent);
  margin-bottom: 12px;
}

.eyebrow {
  font-size: 11px;
  letter-spacing: .32em;
  text-transform: uppercase;
  color: var(--muted);
}

h1 {
  font-family: Georgia, "Times New Roman", serif;
  font-size: clamp(42px, 9vw, 76px);
  line-height: 1.04;
  letter-spacing: .035em;
  margin: 12px 0 10px;
  font-weight: 600;
  text-shadow: 0 8px 35px #000;
}

.subtitle {
  color: #c4c3d1;
  font-size: 14px;
  letter-spacing: .16em;
  text-transform: uppercase;
}

.ruleline {
  width: 90px;
  height: 1px;
  background: linear-gradient(90deg, transparent, var(--accent), transparent);
  margin: 25px auto;
}

.intro {
  max-width: 690px;
  margin: 0 auto 26px;
  text-align: center;
  color: #dedde8;
  font-size: clamp(16px, 3vw, 19px);
}

.intro em {
  color: #c9c8d8;
  font-style: normal;
}

.grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 14px;
}

.card {
  background: linear-gradient(145deg, rgba(39,40,56,.9), rgba(20,21,31,.88));
  border: 1px solid var(--line);
  border-radius: 18px;
  padding: 22px 23px;
  box-shadow: 0 16px 45px rgba(0,0,0,.18);
  backdrop-filter: blur(8px);
}

.card.wide {
  grid-column: 1 / -1;
}

.card h2 {
  font-size: 17px;
  letter-spacing: .075em;
  margin: 0 0 13px;
  display: flex;
  align-items: center;
  gap: 10px;
}

.num {
  font-family: Georgia, serif;
  font-size: 14px;
  color: #bdbcd0;
  border: 1px solid #77778e;
  border-radius: 50%;
  width: 29px;
  height: 29px;
  display: inline-grid;
  place-items: center;
  flex: none;
}

.card ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

.card li {
  position: relative;
  padding-left: 17px;
  margin: 8px 0;
  color: #e1e0e9;
}

.card li:before {
  content: "—";
  position: absolute;
  left: 0;
  color: #aeadc2;
}

.card li:last-child {
  margin-bottom: 0;
}

.note {
  color: var(--muted);
  font-size: 14px;
  margin: 13px 0 0;
}

.penalties {
  margin-top: 18px;
}

.penalties p {
  margin: 7px 0;
  color: #e4e3ec;
}

.warning {
  border-color: rgba(198,177,190,.32);
  background: linear-gradient(145deg, rgba(53,39,53,.75), rgba(22,21,31,.9));
}

.warning h2 {
  color: #e3d3df;
}

.report {
  text-align: center;
  margin-top: 16px;
}

.report h2 {
  justify-content: center;
}

.report p {
  margin: 6px 0;
  color: #e4e3ec;
}

.motto {
  margin: 34px auto 0;
  text-align: center;
  max-width: 680px;
  font-family: Georgia, "Times New Roman", serif;
  font-style: italic;
  font-size: clamp(17px, 3.5vw, 22px);
  color: #d4d2e1;
}

.motto strong {
  display: block;
  font-family: Inter, sans-serif;
  font-style: normal;
  font-size: clamp(15px, 3vw, 18px);
  letter-spacing: .04em;
  margin-top: 18px;
  color: #f1eff7;
}

.footer {
  text-align: center;
  color: #77778d;
  font-size: 11px;
  letter-spacing: .2em;
  margin-top: 34px;
  text-transform: uppercase;
}

@media(max-width:650px) {
  .wrap {
    padding-top: 26px;
  }

  .grid {
    grid-template-columns: 1fr;
  }

  .card.wide {
    grid-column: auto;
  }

  .card {
    padding: 20px;
  }

  .hero {
    padding-bottom: 26px;
  }
}

@media(prefers-reduced-motion:no-preference) {
  .card {
    animation: rise .65s both;
  }

  .card:nth-child(2) {
    animation-delay: .07s;
  }

  .card:nth-child(3) {
    animation-delay: .14s;
  }

  .card:nth-child(4) {
    animation-delay: .21s;
  }

  @keyframes rise {
    from {
      opacity: 0;
      transform: translateY(10px);
    }
    to {
      opacity: 1;
      transform: none;
    }
  }
}
</style>
</head>

<body>

<main class="wrap">

<header class="hero">
  <div class="sigil">✧ 𓆩♡𓆪 ✧</div>

  <div class="eyebrow">
    Добро пожаловать в наш мир
  </div>

  <h1>OMNIX CLAN</h1>

  <div class="subtitle">
    Правила нашего мира
  </div>

  <div class="ruleline"></div>

  <p class="intro">
    Прежде чем войти в наш мир,
    <em>прочтите правила</em>.
    Даже ангелы и демоны обязаны им следовать.
  </p>
</header>

<section class="grid" aria-label="Правила клана">

<article class="card">
  <h2><span class="num">01</span> ОБЩЕНИЕ</h2>
  <ul>
    <li>Уважайте участников и не переходите границы.</li>
    <li>Токсичность, травля, провокации и серьёзные оскорбления запрещены.</li>
    <li>Шутки допустимы, если они не обижают других.</li>
  </ul>
</article>

<article class="card">
  <h2><span class="num">02</span> ПОРЯДОК</h2>
  <ul>
    <li>Не игнорируйте участников и администрацию.</li>
    <li>Не раскрывайте чужие личные данные.</li>
    <li>Реклама и спам запрещены.</li>
    <li>Мат допустим в меру.</li>
  </ul>
</article>

<article class="card">
  <h2><span class="num">03</span> АДМИНИСТРАЦИЯ</h2>
  <ul>
    <li>Обращайтесь к администрации по важным вопросам.</li>
    <li>Не вмешивайтесь в чужие конфликты — позовите модератора.</li>
  </ul>
</article>

<article class="card">
  <h2><span class="num">04</span> КОНТЕНТ</h2>
  <ul>
    <li>Запрещены порнография, эротический и шок-контент.</li>
    <li>Кровавые материалы нежелательны; при публикации скрывайте их под спойлер.</li>
  </ul>
</article>

<article class="card wide">
  <h2><span class="num">05</span> СЪЁМКИ</h2>
  <ul>
    <li>Если в течение недели вы не появляетесь на съёмках, вас автоматически исключат из клана.</li>
  </ul>
</article>

<article class="card wide warning">
  <h2>⚖ НАКАЗАНИЯ</h2>

  <div class="penalties">
    <p><strong>1 нарушение</strong> — предупреждение.</p>
    <p><strong>2 нарушения</strong> — мут или предупреждение.</p>
    <p><strong>3 нарушения</strong> — мут или бан.</p>
    <p><strong>4 нарушения</strong> — бан.</p>
  </div>

  <p class="note">
    <em>Мера наказания зависит от тяжести нарушения.
    За серьёзные проступки бан возможен сразу.</em>
  </p>
</article>

<article class="card wide report">
  <h2>𓆩♡𓆪 ЗАМЕТИЛИ НАРУШЕНИЕ?</h2>
  <p>Сообщите администрации или оставьте жалобу в анонимном чате.</p>
</article>

</section>

<p class="motto">
  Свет не оправдывает гордыню.<br>
  Тьма не оправдывает жестокость.

  <strong>
    ♥ OMNIX CLAN — здесь у каждого свои крылья, но правила едины.
  </strong>
</p>

<footer class="footer">
  OMNIX CLAN · правила для каждого
</footer>

</main>

</body>
</html>
