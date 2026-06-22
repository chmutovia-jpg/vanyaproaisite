# Инструкция деплоя

## Вариант 1 — через браузер

1. Открой GitHub.
2. Нажми `New repository`.
3. Название: например `vanyaproai` или `portfolio`.
4. Сделай репозиторий `Public`.
5. Нажми `Create repository`.
6. Нажми `uploading an existing file`.
7. Перетащи все файлы из этой папки.
8. Нажми `Commit changes`.
9. Открой `Settings → Pages`.
10. В блоке `Build and deployment` выбери:
    - Source: `Deploy from a branch`
    - Branch: `main`
    - Folder: `/ (root)`
11. Нажми `Save`.
12. Подожди пару минут и открой ссылку, которую покажет GitHub Pages.

## Вариант 2 — через терминал

```bash
cd путь/к/папке/vanya_landing_github_version

git init
git add .
git commit -m "Deploy personal landing page"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
git push -u origin main
```

Потом включи Pages:

```txt
Settings → Pages → Deploy from a branch → main → /root → Save
```

## Проверка перед публикацией

- `index.html` лежит в корне репозитория.
- `.nojekyll` лежит в корне репозитория.
- Сайт открывается локально двойным кликом по `index.html`.
