# YouTube Clone

**Пет-проект**: Клон платформы для видео-хостинга YouTube. Этот проект реализует основные функции YouTube, такие как регистрация, аутентификация, загрузка видео, поиск, а также дополнительные возможности, включая стриминг видео, систему рекомендаций, лайки/дизлайки и авторизацию через **OAuth**.

Проект создан для изучения современных технологий, таких как **Go**, **React**, и работы с контейнеризацией и CI/CD.

---

## Цели проекта

- Изучение разработки веб-приложений с использованием **Go** и **React**.
- Реализация сложных бизнес-логик, включая систему ролей, стриминг видео и live chat.
- Применение баз данных **PostgreSQL** и **MongoDB**.
- Настройка контейнеризации через **Docker** и автоматизация деплоя с **GitHub Actions**.

---

## Roles

### Доступные роли:
- **Admin**: Управляет всей системой, может блокировать пользователей, редактировать или удалять видео.
- **Moderator**: Следит за комментариями, модерирует контент и пользователей.
- **User**: Обычный пользователь, который может просматривать видео, подписываться, комментировать и оценивать контент.

---

## Features

### Основные возможности:
1. **Streaming Video**
   - Возможность стриминга видео в реальном времени.
   - Интеграция с протоколами **RTMP** и **WebRTC**.

2. **Live Chat**
   - Общение пользователей во время стримов.
   - Автоматическое обновление сообщений в режиме реального времени.

3. **Подписки**
   - Пользователи могут подписываться на других авторов, чтобы получать уведомления о новых видео и стримах.

4. **Лайки, дизлайки, комментарии**
   - Оценка видео с помощью лайков/дизлайков.
   - Возможность оставлять комментарии, с модерацией для борьбы с неподобающим контентом.

5. **Уведомления**
   - Система уведомлений о новых видео, комментариях или ответах.

6. **Система рекомендаций**
   - Персонализированные рекомендации на основе предпочтений пользователя и истории просмотров.

7. **Авторизация через OAuth**
   - Поддержка авторизации через популярные сервисы, такие как Google, Facebook и GitHub.
   - Упрощенный процесс входа для пользователей через их существующие аккаунты.

---

## Технологический стек

- **Frontend**: React, Redux, TypeScript
- **Backend**: Go
- **Базы данных**:
  - **PostgreSQL**: Хранение информации о пользователях, ролях и видео.
  - **MongoDB**: Хранение метаданных, комментариев и истории просмотров.
  - **Redis**: Используется для кэширования и хранения live chat сообщений.
- **Контейнеризация**: Docker, Docker Compose
- **Message Broker**: Apache Kafka для обработки событий и уведомлений.
- **CI/CD**: GitHub Actions для автоматизации сборки и деплоя.
