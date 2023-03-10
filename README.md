Першим ділом треба надати gradlew права на виконання:

`git update-index --chmod=+x gradlew`

# goit-java-dev-mod16-hw-cicd-git-actions

На **Github** є базовий інструментарій для `CI/CD` процесів. Цей інструмент називається **Github Actions**.

Документацію можна почитати ось тут - [Github Actions docs](https://github.com/features/actions)

Один з варіантів використання **Github Actions** - це коли у гілку **main** відкривається **Pull Request**, то автоматично запускаються **Unit** тести для цієї гілки.

Технічно, це реалізується наступним чином:

ми визначаємо тригер на який необхідно реагувати (у нашому випадку - це відкриття **Pull Request** у гілку **main**)
ми пишемо дію яку необхідно виконати (якщо у нас, наприклад, `gradle` проєкт - то це запуск команди `./gradlew test`)
Офіційний tutorial по запуску тестів для Java за допомогою [Tutorial Github Workflow](https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-java-with-gradle)

## Завдання №1 - налаштуй запуск юніт-тестів для будь-якого проєкту
Візьми будь-який проєкт, де є юніт-тести (якщо такого проєкту немає - то створи новий проєкт, де створи один будь-який юніт-тест).

Налаштуй для цього проєкту **Github Action**, який при **Pull Request** в гілку main запускатиме прогон юніт-тестів. Відкрий один **PR** в гілку main, і переконайсь, що **Github Action** запустивсь.

Результат ДЗ - посилання на **Github** репозиторій з налаштованим **Github Action**.

---

test_branch