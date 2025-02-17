## Hi there 👋

<!--
**Ibrohim1232/Ibrohim1232** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MusicWorld - Ваш музыкальный мир</title>
    <style>
        /* Основные стили */
        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #121212;
            color: #ffffff;
        }
        
        /* Шапка сайта */
        header {
            background-color: #1a1a1a;
            padding: 20px 40px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.3);
        }
        
        .logo {
            display: flex;
            align-items: center;
        }
        
        .logo img {
            height: 50px;
            margin-right: 10px;
        }
        
        .logo h1 {
            font-size: 24px;
            color: #1DB954; /* Зеленый цвет в стиле Spotify */
            margin: 0;
        }
        
        /* Навигация */
        nav ul {
            display: flex;
            list-style: none;
            margin: 0;
            padding: 0;
        }
        
        nav li {
            margin: 0 15px;
        }
        
        nav a {
            color: #b3b3b3;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
        }
        
        nav a:hover {
            color: #1DB954;
        }
        
        /* Основной контент */
        main {
            max-width: 1200px;
            margin: 0 auto;
            padding: 30px 20px;
        }
        
        section {
            margin-bottom: 40px;
        }
        
        h2 {
            color: #ffffff;
            border-bottom: 2px solid #1DB954;
            padding-bottom: 10px;
            margin-bottom: 20px;
        }
        
        /* Секция музыкальных карточек */
        .music-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            gap: 20px;
        }
        
        .music-card {
            background: #2a2a2a;
            border-radius: 8px;
            overflow: hidden;
            transition: transform 0.3s;
            cursor: pointer;
        }
        
        .music-card:hover {
            transform: scale(1.05);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
        }
        
        .music-card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }
        
        .music-card-content {
            padding: 15px;
        }
        
        .music-card h3 {
            margin: 0 0 5px 0;
            font-size: 16px;
        }
        
        .music-card p {
            margin: 0;
            color: #b3b3b3;
            font-size: 14px;
        }
        
        /* Плеер */
        .player {
            background: #282828;
            padding: 15px;
            border-radius: 8px;
            margin-top: 30px;
            display: flex;
            align-items: center;
        }
        
        .player-controls {
            display: flex;
            align-items: center;
            margin-right: 20px;
        }
        
        .player-button {
            background: none;
            border: none;
            color: #b3b3b3;
            font-size: 24px;
            cursor: pointer;
            margin: 0 10px;
            transition: color 0.3s;
        }
        
        .player-button:hover {
            color: #1DB954;
        }
        
        .play-button {
            color: #1DB954;
            background: #ffffff;
            border-radius: 50%;
            width: 40px;
            height: 40px;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .player-info {
            flex-grow: 1;
        }
        
        .progress-bar {
            background: #5a5a5a;
            height: 5px;
            border-radius: 3px;
            margin-top: 5px;
            position: relative;
        }
        
        .progress {
            background: #1DB954;
            height: 100%;
            width: 30%;
            border-radius: 3px;
        }
        
        /* Подвал */
        footer {
            background: #1a1a1a;
            padding: 30px 40px;
        }
        
        .footer-container {
            max-width: 1200px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 30px;
        }
        
        footer h4 {
            color: #ffffff;
            margin-top: 0;
        }
        
        footer ul {
            list-style: none;
            padding: 0;
            margin: 0;
        }
        
        footer li {
            margin-bottom: 10px;
        }
        
        footer a {
            color: #b3b3b3;
            text-decoration: none;
        }
        
        footer a:hover {
            color: #1DB954;
            text-decoration: underline;
        }
        
        .copyright {
            margin-top: 30px;
            text-align: center;
            color: #b3b3b3;
            font-size: 14px;
        }
    </style>
</head>
<body>
    <!-- Шапка сайта -->
    <header>
        <div class="logo">
            <img src="/api/placeholder/50/50" alt="MusicWorld Logo">
            <h1>MusicWorld</h1>
        </div>
        <nav>
            <ul>
                <li><a href="#">Главная</a></li>
                <li><a href="#">Новинки</a></li>
                <li><a href="#">Плейлисты</a></li>
                <li><a href="#">Исполнители</a></li>
                <li><a href="#">Альбомы</a></li>
                <li><a href="#">Радио</a></li>
            </ul>
        </nav>
    </header>
    
    <!-- Основной контент -->
    <main>
        <!-- Секция популярных исполнителей -->
        <section>
            <h2>Популярные исполнители</h2>
            <div class="music-grid">
                <div class="music-card">
                    <img src="/api/placeholder/200/200" alt="Исполнитель 1">
                    <div class="music-card-content">
                        <h3>Татьяна Буланова</h3>
                        <p>Поп-музыка</p>
                    </div>
                </div>
                <div class="music-card">
                    <img src="/api/placeholder/200/200" alt="Исполнитель 2">
                    <div class="music-card-content">
                        <h3>Баста</h3>
                        <p>Хип-хоп</p>
                    </div>
                </div>
                <div class="music-card">
                    <img src="/api/placeholder/200/200" alt="Исполнитель 3">
                    <div class="music-card-content">
                        <h3>Земфира</h3>
                        <p>Рок, Альтернатива</p>
                    </div>
                </div>
                <div class="music-card">
                    <img src="/api/placeholder/200/200" alt="Исполнитель 4">
                    <div class="music-card-content">
                        <h3>Тимати</h3>
                        <p>Рэп</p>
                    </div>
                </div>
                <div class="music-card">
                    <img src="/api/placeholder/200/200" alt="Исполнитель 5">
                    <div class="music-card-content">
                        <h3>Полина Гагарина</h3>
                        <p>Поп-музыка</p>
                    </div>
                </div>
            </div>
        </section>
        
        <!-- Секция новых релизов -->
        <section>
            <h2>Новые релизы</h2>
            <div class="music-grid">
                <div class="music-card">
                    <img src="/api/placeholder/200/200" alt="Альбом 1">
                    <div class="music-card-content">
                        <h3>Новый мир</h3>
                        <p>Артур Пирожков</p>
                    </div>
                </div>
                <div class="music-card">
                    <img src="/api/placeholder/200/200" alt="Альбом 2">
                    <div class="music-card-content">
                        <h3>Лучшие дни</h3>
                        <p>Елена Темникова</p>
                    </div>
                </div>
                <div class="music-card">
                    <img src="/api/placeholder/200/200" alt="Альбом 3">
                    <div class="music-card-content">
                        <h3>Горизонт</h3>
                        <p>Дима Билан</p>
                    </div>
                </div>
                <div class="music-card">
                    <img src="/api/placeholder/200/200" alt="Альбом 4">
                    <div class="music-card-content">
                        <h3>Весна</h3>
                        <p>Ани Лорак</p>
                    </div>
                </div>
            </div>
        </section>
        
        <!-- Плеер -->
        <div class="player">
            <div class="player-controls">
                <button class="player-button">&#8249;&#8249;</button>
                <button class="player-button play-button">▶</button>
                <button class="player-button">&#8250;&#8250;</button>
            </div>
            <div class="player-info">
                <h3>Татьяна Буланова - Не плачь</h3>
                <div class="progress-bar">
                    <div class="progress"></div>
                </div>
            </div>
        </div>
    </main>
    
    <!-- Подвал -->
    <footer>
        <div class="footer-container">
            <div>
                <h4>Компания</h4>
                <ul>
                    <li><a href="#">О нас</a></li>
                    <li><a href="#">Работа у нас</a></li>
                    <li><a href="#">Для бизнеса</a></li>
                    <li><a href="#">Новости</a></li>
                </ul>
            </div>
            <div>
                <h4>Сообщества</h4>
                <ul>
                    <li><a href="#">Для исполнителей</a></li>
                    <li><a href="#">Разработчикам</a></li>
                    <li><a href="#">Рекламодателям</a></li>
                    <li><a href="#">Инвесторам</a></li>
                </ul>
            </div>
            <div>
                <h4>Полезные ссылки</h4>
                <ul>
                    <li><a href="#">Поддержка</a></li>
                    <li><a href="#">Мобильное приложение</a></li>
                    <li><a href="#">Бесплатная версия</a></li>
                </ul>
            </div>
            <div>
                <h4>Юридическая информация</h4>
                <ul>
                    <li><a href="#">Конфиденциальность</a></li>
                    <li><a href="#">Условия использования</a></li>
                    <li><a href="#">Авторское право</a></li>
                    <li><a href="#">Cookies</a></li>
                </ul>
            </div>
        </div>
        <div class="copyright">
            © 2025 MusicWorld. Все права защищены.
        </div>
    </footer>

    <script>
        // Простой скрипт для имитации работы плеера
        document.addEventListener('DOMContentLoaded', function() {
            const playButton = document.querySelector('.play-button');
            let isPlaying = false;
            
            playButton.addEventListener('click', function() {
                if (isPlaying) {
                    playButton.innerHTML = '▶';
                    isPlaying = false;
                } else {
                    playButton.innerHTML = '❚❚';
                    isPlaying = true;
                }
            });
            
            // Имитация обновления прогресс-бара
            const progress = document.querySelector('.progress');
            let width = 30;
            
            setInterval(function() {
                if (isPlaying) {
                    width = (width + 1) % 100;
                    progress.style.width = width + '%';
                }
            }, 1000);
            
            // Интерактивность карточек
            const cards = document.querySelectorAll('.music-card');
            cards.forEach(card => {
                card.addEventListener('click', function() {
                    const title = this.querySelector('h3').textContent;
                    const artist = this.querySelector('p').textContent;
                    document.querySelector('.player-info h3').textContent = artist + ' - ' + title;
                    playButton.innerHTML = '❚❚';
                    isPlaying = true;
                });
            });
        });
    </script>
</body>
</html>
<!-- Страница "Новинки" -->
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Новинки музыки - MusicWorld</title>
    <style>
        /* Основные стили (те же, что и на главной странице) */
        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #121212;
            color: #ffffff;
        }
        
        /* Шапка сайта */
        header {
            background-color: #1a1a1a;
            padding: 20px 40px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.3);
        }
        
        .logo {
            display: flex;
            align-items: center;
        }
        
        .logo img {
            height: 50px;
            margin-right: 10px;
        }
        
        .logo h1 {
            font-size: 24px;
            color: #1DB954;
            margin: 0;
        }
        
        /* Навигация */
        nav ul {
            display: flex;
            list-style: none;
            margin: 0;
            padding: 0;
        }
        
        nav li {
            margin: 0 15px;
        }
        
        nav a {
            color: #b3b3b3;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
        }
        
        nav a:hover, nav a.active {
            color: #1DB954;
        }
        
        /* Основной контент */
        main {
            max-width: 1200px;
            margin: 0 auto;
            padding: 30px 20px;
        }
        
        section {
            margin-bottom: 40px;
        }
        
        h2 {
            color: #ffffff;
            border-bottom: 2px solid #1DB954;
            padding-bottom: 10px;
            margin-bottom: 20px;
        }
        
        /* Секция музыкальных карточек */
        .music-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            gap: 20px;
        }
        
        .music-card {
            background: #2a2a2a;
            border-radius: 8px;
            overflow: hidden;
            transition: transform 0.3s;
            cursor: pointer;
        }
        
        .music-card:hover {
            transform: scale(1.05);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
        }
        
        .music-card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }
        
        .music-card-content {
            padding: 15px;
        }
        
        .music-card h3 {
            margin: 0 0 5px 0;
            font-size: 16px;
        }
        
        .music-card p {
            margin: 0;
            color: #b3b3b3;
            font-size: 14px;
        }
        
        /* Плеер */
        .player {
            background: #282828;
            padding: 15px;
            border-radius: 8px;
            margin-top: 30px;
            display: flex;
            align-items: center;
            position: fixed;
            bottom: 20px;
            left: 20px;
            right: 20px;
            max-width: 1200px;
            margin-left: auto;
            margin-right: auto;
            box-shadow: 0 -2px 10px rgba(0, 0, 0, 0.3);
        }
        
        .player-controls {
            display: flex;
            align-items: center;
            margin-right: 20px;
        }
        
        .player-button {
            background: none;
            border: none;
            color: #b3b3b3;
            font-size: 24px;
            cursor: pointer;
            margin: 0 10px;
            transition: color 0.3s;
        }
        
        .player-button:hover {
            color: #1DB954;
        }
        
        .play-button {
            color: #1DB954;
            background: #ffffff;
            border-radius: 50%;
            width: 40px;
            height: 40px;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .player-info {
            flex-grow: 1;
        }
        
        .progress-bar {
            background: #5a5a5a;
            height: 5px;
            border-radius: 3px;
            margin-top: 5px;
            position: relative;
        }
        
        .progress {
            background: #1DB954;
            height: 100%;
            width: 30%;
            border-radius: 3px;
        }
        
        /* Подвал */
        footer {
            background: #1a1a1a;
            padding: 30px 40px;
            margin-top: 80px;
        }
        
        .footer-container {
            max-width: 1200px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 30px;
        }
        
        footer h4 {
            color: #ffffff;
            margin-top: 0;
        }
        
        footer ul {
            list-style: none;
            padding: 0;
            margin: 0;
        }
        
        footer li {
            margin-bottom: 10px;
        }
        
        footer a {
            color: #b3b3b3;
            text-decoration: none;
        }
        
        footer a:hover {
            color: #1DB954;
            text-decoration: underline;
        }
        
        .copyright {
            margin-top: 30px;
            text-align: center;
            color: #b3b3b3;
            font-size: 14px;
        }
        
        /* Стили для новинок */
        .new-releases-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 30px;
        }
        
        .filter-dropdown {
            background: #2a2a2a;
            border: none;
            color: #ffffff;
            padding: 8px 15px;
            border-radius: 4px;
            font-size: 14px;
            cursor: pointer;
        }
        
        .release-date {
            color: #b3b3b3;
            font-size: 12px;
            margin-top: 5px;
        }
        
        .featured-release {
            display: grid;
            grid-template-columns: 1fr 2fr;
            background: #2a2a2a;
            border-radius: 8px;
            overflow: hidden;
            margin-bottom: 30px;
        }
        
        .featured-release img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        
        .featured-content {
            padding: 30px;
        }
        
        .featured-content h3 {
            font-size: 24px;
            margin: 0 0 10px 0;
        }
        
        .featured-content p {
            color: #b3b3b3;
            margin-bottom: 20px;
        }
        
        .listen-button {
            background: #1DB954;
            color: #ffffff;
            border: none;
            padding: 10px 20px;
            border-radius: 20px;
            font-weight: bold;
            cursor: pointer;
            transition: background 0.3s;
        }
        
        .listen-button:hover {
            background: #169c46;
        }
    </style>
</head>
<body>
    <!-- Шапка сайта -->
    <header>
        <div class="logo">
            <img src="/api/placeholder/50/50" alt="MusicWorld Logo">
            <h1>MusicWorld</h1>
        </div>
        <nav>
            <ul>
                <li><a href="index.html">Главная</a></li>
                <li><a href="new-releases.html" class="active">Новинки</a></li>
                <li><a href="playlists.html">Плейлисты</a></li>
                <li><a href="artists.html">Исполнители</a></li>
                <li><a href="albums.html">Альбомы</a></li>
                <li><a href="#">Радио</a></li>
            </ul>
        </nav>
    </header>
    
    <!-- Основной контент -->
    <main>
        <div class="new-releases-header">
            <h2>Новинки этой недели</h2>
            <select class="filter-dropdown">
                <option>Все жанры</option>
                <option>Поп</option>
                <option>Рок</option>
                <option>Хип-хоп</option>
                <option>Электронная</option>
                <option>Классическая</option>
            </select>
        </div>
        
        <!-- Главный релиз недели -->
        <div class="featured-release">
            <img src="/api/placeholder/400/400" alt="Главный релиз недели">
            <div class="featured-content">
                <h3>Новый альбом группы "Звуки Моря"</h3>
                <p class="release-date">Выпущен: 15 февраля 2025</p>
                <p>Долгожданный альбом культовой группы "Звуки Моря" с новым звучанием и неожиданными коллаборациями. 12 новых треков, записанных на легендарной студии.</p>
                <button class="listen-button">Слушать сейчас</button>
            </div>
        </div>
        
        <!-- Новые синглы -->
        <section>
            <h2>Новые синглы</h2>
            <div class="music-grid">
                <div class="music-card">
                    <img src="/api/placeholder/200/200" alt="Новый сингл 1">
                    <div class="music-card-content">
                        <h3>Летний закат</h3>
                        <p>Алексей Петров</p>
                        <p class="release-date">14 февраля 2025</p>
                    </div>
                </div>
                <div class="music-card">
                    <img src="/api/placeholder/200/200" alt="Новый сингл 2">
                    <div class="music-card-content">
                        <h3>Невидимые нити</h3>
                        <p>Мария Волкова</p>
                        <p class="release-date">14 февраля 2025</p>
                    </div>
                </div>
                <div class="music-card">
                    <img src="/api/placeholder/200/200" alt="Новый сингл 3">
                    <div class="music-card-content">
                        <h3>Глубокий океан</h3>
                        <p>Группа "Волны"</p>
                        <p class="release-date">13 февраля 2025</p>
                    </div>
                </div>
                <div class="music-card">
                    <img src="/api/placeholder/200/200" alt="Новый сингл 4">
                    <div class="music-card-content">
                        <h3>Последний поезд</h3>
                        <p>Алёна Морозова</p>
                        <p class="release-date">12 февраля 2025</p>
                    </div>
                </div>
            </div>
        </section>
        
        <!-- Новые альбомы -->
        <section>
            <h2>Новые альбомы</h2>
            <div class="music-grid">
                <div class="music-card">
                    <img src="/api/placeholder/200/200" alt="Новый альбом 1">
                    <div class="music-card-content">
                        <h3>Вечные истории</h3>
                        <p>Группа "Странники"</p>
                        <p class="release-date">10 февраля 2025</p>
                    </div>
                </div>
                <div class="music-card">
                    <img src="/api/placeholder/200/200" alt="Новый альбом 2">
                    <div class="music-card-content">
                        <h3>Мечты о будущем</h3>
                        <p>Иван Соколов</p>
                        <p class="release-date">8 февраля 2025</p>
                    </div>
                </div>
                <div class="music-card">
                    <img src="/api/placeholder/200/200" alt="Новый альбом 3">
                    <div class="music-card-content">
                        <h3>Космические путешествия</h3>
                        <p>Электроника 2.0</p>
                        <p class="release-date">5 февраля 2025</p>
                    </div>
                </div>
                <div class="music-card">
                    <img src="/api/placeholder/200/200" alt="Новый альбом 4">
                    <div class="music-card-content">
                        <h3>Тихие вечера</h3>
                        <p>Елена Светлая</p>
                        <p class="release-date">3 февраля 2025</p>
                    </div>
                </div>
            </div>
        </section>
        
        <!-- Плеер -->
        <div class="player">
            <div class="player-controls">
                <button class="player-button">&#8249;&#8249;</button>
                <button class="player-button play-button">▶</button>
                <button class="player-button">&#8250;&#8250;</button>
            </div>
            <div class="player-info">
                <h3>Выберите трек для прослушивания</h3>
                <div class="progress-bar">
                    <div class="progress"></div>
                </div>
            </div>
        </div>
    </main>
    
    <!-- Подвал -->
    <footer>
        <div class="footer-container">
            <div>
                <h4>Компания</h4>
                <ul>
                    <li><a href="#">О нас</a></li>
                    <li><a href="#">Работа у нас</a></li>
                    <li><a href="#">Для бизнеса</a></li>
                    <li><a href="#">Новости</a></li>
                </ul>
            </div>
            <div>
                <h4>Сообщества</h4>
                <ul>
                    <li><a href="#">Для исполнителей</a></li>
                    <li><a href="#">Разработчикам</a></li>
                    <li><a href="#">Рекламодателям</a></li>
                    <li><a href="#">Инвесторам</a></li>
                </ul>
            </div>
            <div>
                <h4>Полезные ссылки</h4>
                <ul>
                    <li><a href="#">Поддержка</a></li>
                    <li><a href="#">Мобильное приложение</a></li>
                    <li><a href="#">Бесплатная версия</a></li>
                </ul>
            </div>
            <div>
                <h4>Юридическая информация</h4>
                <ul>
                    <li><a href="#">Конфиденциальность</a></li>
                    <li><a href="#">Условия использования</a></li>
                    <li><a href="#">Авторское право</a></li>
                    <li><a href="#">Cookies</a></li>
                </ul>
            </div>
        </div>
        <div class="copyright">
            © 2025 MusicWorld. Все права защищены.
        </div>
    </footer>

    <script>
        // Простой скрипт для имитации работы плеера
        document.addEventListener('DOMContentLoaded', function() {
            const playButton = document.querySelector('.play-button');
            let isPlaying = false;
            
            playButton.addEventListener('click', function() {
                if (isPlaying) {
                    playButton.innerHTML = '▶';
                    isPlaying = false;
                } else {
                    playButton.innerHTML = '❚❚';
                    isPlaying = true;
                }
            });
            
            // Имитация обновления прогресс-бара
            const progress = document.querySelector('.progress');
            let width = 30;
            
            setInterval(function() {
                if (isPlaying) {
                    width = (width + 1) % 100;
                    progress.style.width = width + '%';
                }
            }, 1000);
            
            // Интерактивность карточек
            const cards = document.querySelectorAll('.music-card');
            cards.forEach(card => {
                card.addEventListener('click', function() {
                    const title = this.querySelector('h3').textContent;
                    const artist = this.querySelector('p').textContent;
                    document.querySelector('.player-info h3').textContent = artist + ' - ' + title;
                    playButton.innerHTML = '❚❚';
                    isPlaying = true;
                });
            });
            
            // Обработка клика на "Слушать сейчас"
            const listenButton = document.querySelector('.listen-button');
            if (listenButton) {
                listenButton.addEventListener('click', function() {
                    const featuredRelease = document.querySelector('.featured-release');
                    const title = featuredRelease.querySelector('h3').textContent;
                    document.querySelector('.player-info h3').textContent = title;
                    playButton.innerHTML = '❚❚';
                    isPlaying = true;
                });
            }
        });
    </script>
</body>
</html>

<!-- Страница "Плейлисты" -->
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Плейлисты - MusicWorld</title>
    <style>
        /* Основные стили (те же, что и на главной странице) */
        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #121212;
            color: #ffffff;
        }
        
        /* Шапка сайта */
        header {
            background-color: #1a1a1a;
            padding: 20px 40px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.3);
        }
        
        .logo {
            display: flex;
            align-items: center;
        }
        
        .logo img {
            height: 50px;
            margin-right: 10px;
        }
        
        .logo h1 {
            font-size: 24px;
            color: #1DB954;
            margin: 0;
        }
        
        /* Навигация */
        nav ul {
            display: flex;
            list-style: none;
            margin: 0;
            padding: 0;
        }
        
        nav li {
            margin: 0 15px;
        }
        
        nav a {
            color: #b3b3b3;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
        }
        
        nav a:hover, nav a.active {
            color: #1DB954;
        }
        
        /* Основной контент */
        main {
            max-width: 1200px;
            margin: 0 auto;
            padding: 30px 20px;
        }
        
        section {
            margin-bottom: 40px;
        }
        
        h2 {
            color: #ffffff;
            border-bottom: 2px solid #1DB954;
            padding-bottom: 10px;
            margin-bottom: 20px;
        }
        
        /* Секция музыкальных карточек */
        .music-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            gap: 20px;
        }
        
        .music-card {
            background: #2a2a2a;
            border-radius: 8px;
            overflow: hidden;
            transition: transform 0.3s;
            cursor: pointer;
        }
        
        .music-card:hover {
            transform: scale(1.05);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
        }
        
        .music-card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }
        
        .music-card-content {
            padding: 15px;
        }
        
        .music-card h3 {
            margin: 0 0 5px 0;
            font-size: 16px;
        }
        
        .music-card p {
            margin: 0;
            color: #b3b3b3;
            font-size: 14px;
        }
        
        /* Плеер */
        .player {
            background: #282828;
            padding: 15px;
            border-radius: 8px;
            margin-top: 30px;
            display: flex;
            align-items: center;
            position: fixed;
            bottom: 20px;
            left: 20px;
            right: 20px;
            max-width: 1200px;
            margin-left: auto;
            margin-right: auto;
            box-shadow: 0 -2px 10px rgba(0, 0, 0, 0.3);
        }
        
        .player-controls {
            display: flex;
            align-items: center;
            margin-right: 20px;
        }
        
        .player-button {
            background: none;
            border: none;
            color: #b3b3b3;
            font-size: 24px;
            cursor: pointer;
            margin: 0 10px;
            transition: color 0.3s;
        }
        
        .player-button:hover {
            color: #1DB954;
        }
        
        .play-button {
            color: #1DB954;
            background: #ffffff;
            border-radius: 50%;
            width: 40px;
            height: 40px;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .player-info {
            flex-grow: 1;
        }
        
        .progress-bar {
            background: #5a5a5a;
            height: 5px;
            border-radius: 3px;
            margin-top: 5px;
            position: relative;
        }
        
        .progress {
            background: #1DB954;
            height: 100%;
            width: 30%;
            border-radius: 3px;
        }
        
        /* Подвал */
        footer {
            background: #1a1a1a;
            padding: 30px 40px;
            margin-top: 80px;
        }
        
        .footer-container {
            max-width: 1200px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 30px;
        }
        
        footer h4 {
            color: #ffffff;
            margin-top: 0;
        }
        
        footer ul {
            list-style: none;
            padding: 0;
            margin: 0;
        }
        
        footer li {
            margin-bottom: 10px;
        }
        
        footer a {
            color: #b3b3b3;
            text-decoration: none;
        }
        
        footer a:hover {
            color: #1DB954;
            text-decoration: underline;
        }
        
        .copyright {
            margin-top: 30px;
            text-align: center;
            color: #b3b3b3;
            font-size: 14px;
        }
        
        /* Стили для плейлистов */
        .tabs {
            display: flex;
            border-bottom: 1px solid #333;
            margin-bottom: 30px;
        }
        
        .tab {
            padding: 10px 20px;
            cursor: pointer;
            color: #b3b3b3;
            transition: all 0.3s;
        }
        
        .tab.active {
            color: #ffffff;
            border-bottom: 2px solid #1DB954;
        }
        
        .playlist-description {
            color: #b3b3b3;
            font-size: 14px;
            margin-top: 5px;
            line-height: 1.4;
        }
        
        .playlist-stats {
            display: flex;
            margin-top: 10px;
            color: #888;
            font-size: 12px;
        }
        
        .playlist-stats span {
            margin-right: 15px;
        }
        
        .create-playlist {
            background: transparent;
            border: 2px dashed #555;
            border-radius: 8px;
            height: 200px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            transition: all 0.3s;
        }
        
        .create-playlist:hover {
            border-color: #1DB954;
            background: rgba(29, 185, 84, 0.1);
        }
        
        .create-playlist-icon {
            font-size: 48px;
            color: #888;
            margin-bottom: 10px;
        }
        
        .create-playlist-text {
            color: #b3b3b3;
            font-weight: 500;
        }
        
        .featured-playlist {
            background: linear-gradient(to right, #1DB954, #067242);
            padding: 30px;
            border-radius: 8px;
            margin-bottom: 30px;
        }
        
        .featured-playlist h3 {
            font-size: 24px;
            margin: 0 0 10px 0;
        }
        
        .featured-playlist p {
            color: rgba(255, 255, 255, 0.8);
        }
        
        .featured-playlist-button {
            background: rgba(0, 0, 0, 0.3);
            color: #ffffff;
            border: none;
            padding: 8px 20px;
            border-radius: 20px;
            margin-top: 15px;
            cursor: pointer;
            transition: background 0.3s;
        }
        
        .featured-playlist-button:hover {
            background: rgba(0, 0, 0, 0.5);
        }
    </style>
</head>
<body>
    <!-- Шапка сайта -->
    <header>
        <div class="logo">
            <img src="/api/placeholder/50/50" alt="MusicWorld Logo">
            <h1>MusicWorld</h1>
        </div>
        <nav>
            <ul>
                <li><a href="index.html">Главная</a></li>
                <li><a href="new-releases.html">Новинки</a></li>
                <li><a href="playlists.html" class="active">Плейлисты</a></li>
                <li><a href="artists.html">Исполнители</a></li>
                <li><a href="albums.html">Альбомы</a></li>
                <li><a href="#">Радио</a></li>
            </ul>
        </nav>
    </header>
    
    <!-- Основной контент -->
    <main>
        <div class="tabs">
            <div class="tab active">Рекомендации</div>
            <div class="tab">Мои плейлисты</div>
            <div class="tab">По жанрам</div>
            <div class="tab">По настроению</div>
            <div class="tab">Популярные</div>
        </div>
        
        <!-- Избранный плейлист -->
        <div class="featured-playlist">
            <h3>Плейлист недели: Русский Рок</h3>
            <p>Коллекция лучших хитов русского рока всех времен: от классики до современных исполнителей.</p>
            <button class="featured-playlist-button">Слушать сейчас</button>
        </div>
        
        <!-- Ваши плейлисты -->
        <section>
            <h2>Ваши плейлисты</h2>
            <div class="music-grid">
                <div class="music-card">
                    <img src="/api/placeholder/200/200" alt="Плейлист 1">
                    <div class="music-card-content">
                        <h3>Мои любимые</h3>
                        <p class="playlist-![IMG_20250214_201321_559](https://github.com/user-attachments/assets/08205537-d3ce-49c5-be14-47bc9a8fbaa1)
![askai_251557](https://github.com/user-attachments/assets/e59d98cf-87c2-4666-b61a-cef278ee9a52)
