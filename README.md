# -<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>LOGOFLOW — Простой стиль. Сильный эффект.</title>
  <style>
    :root {
      --blue: #0d2b61;
      --lightblue: #4ea4ff;
      --gray: #888;
      --font-main: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;

      --bg-light: #fff;
      --text-light: #0f1117;
      --tile-light: #f4f4f4;
      --footer-light: #0f1117;
      --footer-text-light: #fff;

      --bg-dark: #0f1117;
      --text-dark: #fff;
      --tile-dark: #1a1a1a;
      --footer-dark: #fff;
      --footer-text-dark: #0f1117;
    }

    body {
      margin: 0;
      font-family: var(--font-main);
      background-color: var(--bg-light);
      color: var(--text-light);
      transition: background-color 0.3s, color 0.3s;
      line-height: 1.5;
    }

    body.dark {
      background-color: var(--bg-dark);
      color: var(--text-dark);
    }

    header {
      padding: 60px 20px;
      text-align: center;
    }

    header h1 {
      font-size: 64px;
      color: var(--blue);
      margin: 0 0 10px;
    }

    header p {
      font-size: 22px;
      color: var(--gray);
      margin: 0;
    }

    a.button {
      display: inline-block;
      margin-top: 20px;
      padding: 12px 28px;
      background-color: var(--blue);
      color: #fff;
      text-decoration: none;
      border-radius: 8px;
      font-weight: 600;
      transition: background-color 0.3s;
    }

    a.button:hover {
      background-color: var(--lightblue);
    }

    section {
      max-width: 1100px;
      margin: 40px auto;
      padding: 0 20px;
    }

    h2 {
      text-align: center;
      font-size: 36px;
      margin-bottom: 30px;
      color: var(--blue);
    }

    .tiles {
      display: flex;
      flex-wrap: wrap;
      gap: 30px;
      justify-content: center;
    }

    .tile {
      background-color: var(--tile-light);
      padding: 30px 20px;
      border-radius: 14px;
      flex: 1 1 280px;
      box-shadow: 0 5px 15px rgba(0,0,0,0.05);
      transition: transform 0.3s;
    }

    body.dark .tile {
      background-color: var(--tile-dark);
      box-shadow: 0 5px 15px rgba(255,255,255,0.05);
    }

    .tile:hover {
      transform: translateY(-8px);
    }

    .tile h3 {
      margin-top: 0;
      margin-bottom: 12px;
      color: var(--blue);
    }

    .portfolio {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
      justify-content: center;
    }

    .portfolio img {
      width: 300px;
      height: 200px;
      object-fit: cover;
      border-radius: 10px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
      transition: transform 0.3s;
    }

    .portfolio img:hover {
      transform: scale(1.05);
    }

    ol {
      max-width: 600px;
      margin: 0 auto;
      padding-left: 20px;
    }

    ol li {
      margin-bottom: 15px;
      font-size: 18px;
    }

    section p {
      max-width: 600px;
      margin: 0 auto 10px;
      font-size: 18px;
      color: var(--gray);
      text-align: center;
    }

    footer {
      background-color: var(--footer-light);
      color: var(--footer-text-light);
      text-align: center;
      padding: 25px 10px;
      font-size: 14px;
      user-select: none;
      transition: background-color 0.3s, color 0.3s;
    }

    body.dark footer {
      background-color: var(--footer-dark);
      color: var(--footer-text-dark);
    }

    .theme-toggle {
      position: fixed;
      top: 20px;
      right: 20px;
      background: none;
      border: 2px solid var(--blue);
      color: var(--blue);
      font-size: 20px;
      padding: 8px 14px;
      border-radius: 10px;
      cursor: pointer;
      user-select: none;
      transition: background-color 0.3s, color 0.3s;
      z-index: 1000;
    }

    .theme-toggle:hover {
      background-color: var(--blue);
      color: #fff;
    }

    @media (max-width: 650px) {
      header h1 {
        font-size: 42px;
      }
      h2 {
        font-size: 28px;
      }
      .tiles, .portfolio {
        flex-direction: column;
        align-items: center;
      }
      .tile {
        width: 90%;
      }
      .portfolio img {
        width: 90%;
        height: auto;
      }
    }
  </style>
</head>
<body>

  <button class="theme-toggle" id="themeToggle" aria-label="Переключить тему" title="Переключить тему">🌙</button>

  <header>
    <h1>LOGOFLOW</h1>
    <p>Простой стиль. Сильный эффект.</p>
    <a href="https://t.me/LogoFlow_official" target="_blank" rel="noopener" class="button">Связаться в Telegram</a>
  </header>

  <section>
    <h2>Услуги</h2>
    <div class="tiles">
      <div class="tile">
        <h3>Логотипы</h3>
        <p>Уникальные, запоминающиеся и стильные логотипы, которые отражают характер вашего бренда.</p>
      </div>
      <div class="tile">
        <h3>Аватарки</h3>
        <p>Яркие и современные аватарки для соцсетей, YouTube, Discord и других платформ.</p>
      </div>
      <div class="tile">
        <h3>Фирменный стиль</h3>
        <p>Разработка цветовой палитры, шрифтов и визуального образа для вашего бизнеса или проекта.</p>
      </div>
    </div>
  </section>

  <section>
    <h2>Портфолио</h2>
    <div class="portfolio">
      <img src="https://via.placeholder.com/300x200?text=Пример+1" alt="Пример работы 1" />
      <img src="https://via.placeholder.com/300x200?text=Пример+2" alt="Пример работы 2" />
      <img src="https://via.placeholder.com/300x200?text=Пример+3" alt="Пример работы 3" />
    </div>
  </section>

  <section>
    <h2>Как это работает</h2>
    <ol>
      <li>Вы рассказываете, что хотите и какие идеи у вас есть.</li>
      <li>Я разрабатываю концепт и отправляю вам на согласование.</li>
      <li>Вносим правки, пока не будет идеальный результат.</li>
      <li>Вы получаете финальный дизайн и все файлы.</li>
    </ol>
  </section>

  <section>
    <h2>Отзывы клиентов</h2>
    <p>“Очень доволен логотипом — всё сделано быстро и качественно!”</p>
    <p>“Аватарка просто огонь, теперь профиль выглядит супер профессионально.”</p>
  </section>

  <section>
    <h2>Контакты</h2>
    <p>Связаться со мной можно через Telegram:</p>
    <p><strong>@LogoFlow_official</strong></p>
    <a href="https://t.me/LogoFlow_official" target="_blank" rel="noopener" class="button">Написать в Telegram</a>
  </section>

  <footer>
    © 2025 LOGOFLOW. Все права защищены.
  </footer>

  <script>
    const themeToggle = document.getElementById('themeToggle');
    const body = document.body;

    function setTheme(theme) {
      if (theme === 'dark') {
        body.classList.add('dark');
        themeToggle.textContent = '☀️';
      } else {
        body.classList.remove('dark');
        themeToggle.textContent = '🌙';
      }
      localStorage.setItem('theme', theme);
    }

    themeToggle.addEventListener('click', () => {
      const newTheme = body.classList.contains('dark') ? 'light' : 'dark';
      setTheme(newTheme);
    });

    // Загружаем тему из локального хранилища
    const savedTheme = localStorage.getItem('theme') || 'light';
    setTheme(savedTheme);
  </script>
</body>
</html>
