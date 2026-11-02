# Сайт-портфолио Марии Малявки

Статический сайт + админка для правки текста и фото с телефона и компьютера.

## Запуск (один раз, ~10 минут)

1. На github.com создайте **новый репозиторий** (например `portfolio`), публичный.
2. Загрузите в него **все файлы из этого архива** (Add file → Upload files; папки `admin`, `content`, `images` тоже). Файл `.nojekyll` тоже должен попасть.
3. Откройте `admin/config.yml` в репозитории (карандаш ✏️) и замените
   `YOUR_USERNAME/YOUR_REPO` на свой, например `maryia/portfolio`. Сохраните (Commit).
4. Settings → Pages → Source: **Deploy from a branch**, ветка `main`, папка `/ (root)` → Save.
   Через 1–2 минуты сайт будет на `https://ЛОГИН.github.io/portfolio/`.
5. Создайте токен для входа в админку: github.com → Settings → Developer settings →
   Personal access tokens → **Fine-grained tokens** → Generate new token:
   - Repository access: Only select repositories → ваш репозиторий
   - Permissions → Repository permissions → **Contents: Read and write**
   - Скопируйте токен и сохраните в надёжном месте (в менеджере паролей).

## Как менять сайт

1. Откройте `https://ЛОГИН.github.io/portfolio/admin/` (с телефона или компьютера).
2. Нажмите **Sign in with token**, вставьте токен (на устройстве он запоминается).
3. Раздел «Сайт» → правьте тексты, меняйте фото (кнопка «Выбрать изображение» → загрузить из галереи телефона),
   добавляйте и удаляйте фото в галерее.
4. Нажмите **Save**. Через ~1 минуту изменения появятся на сайте.

## Что где лежит

- `index.html` — сайт (дизайн, менять не нужно)
- `content/site.json` — все тексты и ссылки на фото (его правит админка)
- `images/uploads/` — загруженные фото
- `admin/` — админка (Sveltia CMS)

## Советы

- Перед загрузкой уменьшайте фото до ~2000 px по длинной стороне (JPG, до 500 КБ–1 МБ): сайт будет быстрее.
- Заявки из формы: впишите Telegram-логин в админке (заявка откроется в Telegram) или адрес формы Formspree (заявки на почту).
- Свой домен: Settings → Pages → Custom domain.
