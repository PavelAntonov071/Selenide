[![Build status](https://ci.appveyor.com/api/projects/status/wk7td059geu6f1an?svg=true)](https://ci.appveyor.com/project/Ekaterina5885/dz-2-2-selenide)

## Домашнее задание к занятию «2.2. Selenide»

### Задача - Заказ доставки карты

---

Вам необходимо автоматизировать тестирование формы заказа доставки карты:


![order (1)](https://user-images.githubusercontent.com/82658524/175645641-ca161e04-8393-4ba9-92eb-ff3dfaebaa50.png)

Требования к содержимому полей:

1. Город - один из административных центров субъектов РФ
2. Дата - не ранее трёх дней с текущей даты
3. Поле Фамилия и имя - разрешены только русские буквы, дефисы и пробелы
4. Поле телефон - только цифры (11 цифр), символ + (на первом месте)
5. Флажок согласия должен быть выставлен

Тестируемая функциональность: отправка формы.

Поля Город и Дата заполняются через прямой ввод значений (без использования выбора из выпадающего списка и всплывающего календаря).

Условия: если все поля заполнены корректно, то форма переходит в состояние "Загрузки":


![loading](https://user-images.githubusercontent.com/82658524/175646001-faa55cfb-e99e-4e69-af6d-960c84df50f2.png)

Важно: состояние загрузки не должно длиться более 15 секунд.

После успешной отправки формы (завершения бронирования) появится всплывающее окно об успешном завершении бронирования:

![popup](https://user-images.githubusercontent.com/82658524/175646121-b00599da-cdce-4ec8-b7e4-96720d5c88da.png)

Вам необходимо самостоятельно изучить элементы на странице, чтобы подобрать правильные селекторы. Обратите внимание, что элементы могут быть как скрыты, так и динамически добавляться/удаляться из DOM.
