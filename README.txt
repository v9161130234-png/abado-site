abado website, ready to publish (static site: plain HTML, no build step)
=======================================================================

STRUCTURE
  index.html          English page (site root:  https://your-domain/)
  ru/index.html       Russian page              (https://your-domain/ru/)
  assets/video/       Film in English and Russian (MP4, H.264 + AAC) and poster frames
  assets/shots/en|ru/ App screenshots in each language
  assets/fonts/       Inter, self-hosted (Latin + Cyrillic), no Google Fonts needed. Licence: OFL.txt
  assets/icons/       favicon.ico, SVG icon, apple-touch-icon, Android icon
  assets/og/          Social preview images 1200x630 (EN and RU)

Both pages have an EN/RU switch, and each switches the text, the screenshots and the film.

BEFORE PUBLISHING (3 things)
  1. Contacts. In BOTH index.html and ru/index.html, replace:
       https://t.me/TELEGRAM_USERNAME   with your Telegram link
       mailto:EMAIL@YOUR-DOMAIN.ru      with your email
  2. Social previews. Replace og:image with absolute URLs, for example
       https://your-domain/assets/og/og-en.jpg   (English page)
       https://your-domain/assets/og/og-ru.jpg   (Russian page)
     and, if you want, make the hreflang links absolute too.
  3. Upload the whole folder as is (keep the folder structure). Any static hosting works:
     Yandex Cloud Object Storage, Selectel, Timeweb, Beget, Netlify, nginx and so on.
     If your server compresses files, compress .html/.css only, not .mp4.

To make Russian the default for the whole site, move ru/index.html to the root
and change every "../assets/" in it to "assets/".

------------------------------------------------------------------------
Сайт abado, готов к публикации (статический сайт: обычный HTML, без сборки)

СТРУКТУРА
  index.html          Английская версия (корень сайта)
  ru/index.html       Русская версия (https://ваш-домен/ru/)
  assets/video/       Ролик на русском и английском, обложки
  assets/shots/en|ru/ Скриншоты приложения на двух языках
  assets/fonts/       Шрифт Inter со своего сервера (латиница и кириллица), Google Fonts не нужен
  assets/icons/       Иконки сайта (favicon и др.)
  assets/og/          Картинки для превью в соцсетях и мессенджерах (1200x630)

ПЕРЕД ПУБЛИКАЦИЕЙ
  1. Контакты: в index.html и ru/index.html замените
       https://t.me/TELEGRAM_USERNAME  на вашу ссылку в Telegram
       mailto:EMAIL@YOUR-DOMAIN.ru     на ваш email
  2. Превью: укажите полный адрес картинки og:image, например https://ваш-домен/assets/og/og-ru.jpg
  3. Загрузите папку целиком, сохранив структуру, на любой статический хостинг.

Чтобы русская версия открывалась по умолчанию, перенесите ru/index.html в корень
и замените в нём все "../assets/" на "assets/".
