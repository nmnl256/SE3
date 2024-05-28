# SE3

## Описание системы
Спроектированное приложение позволяет пользователям заказывать еду из множества ресторанов в одном приложении.

## Основные сценарии использования
- **Просмотр меню ресторанов**: Пользователи могут искать рестораны, просматривать их меню и выбирать понравившиеся блюда.
- **Оформление заказа**: Пользователи добавляют выбранные блюда в корзину и оформляют заказ.
- **Оплата заказа**: Пользователи могут оплачивать заказы через интегрированные платежные системы.

## Процесс заказа
1. Пользователь выбирает ресторан.
2. Пользователь добавляет блюда в корзину.
3. Пользователь оформляет и оплачивает заказ.
4. После успешной оплаты ресторан получает уведомление и начинает готовить заказ.
5. Курьер забирает готовый заказ и доставляет его пользователю.

## Состояния заказа
- **Ожидание оплаты**: Заказ создан, ожидается оплата.
- **Оплачен**: Оплата успешно завершена.
- **Подтвержден**: Ресторан подтвердил получение заказа.
- **Готовится**: Ресторан готовит заказ.
- **В пути**: Курьер забрал заказ и везет его к пользователю.
- **Доставлен**: Заказ доставлен пользователю.
- **Отменен**: Заказ отменен (возможные причины: отмена рестораном).


## Диаграмма возможных вариантов использования

<img width="642" alt="Снимок экрана 2024-05-28 в 22 28 41" src="https://github.com/nmnl256/SE3/assets/148970482/27a3d016-dc6b-42af-880d-fba47af703ea">

## Диаграмма последовательности для процесса заказа еды через приложение

<img width="642" alt="Снимок экрана 2024-05-28 в 22 29 04" src="https://github.com/nmnl256/SE3/assets/148970482/1d99c462-45f6-4545-9e12-12a35e7af0c3">



## Диаграмма состояний для заказа 

<img width="634" alt="Снимок экрана 2024-05-28 в 22 37 01" src="https://github.com/nmnl256/SE3/assets/148970482/7cfaa5f3-2f45-4d91-b278-10fc893727b0">

Заказ пользователя может быть отменен, если его не подтвердит ресторан. В случае неуспешной оплаты, будет предложено оплатить заказ повторно.


## Диаграмма деятельности для описания процесса обработки заказа системой

<img width="1067" alt="Снимок экрана 2024-05-28 в 22 39 00" src="https://github.com/nmnl256/SE3/assets/148970482/500eaa76-089f-4158-b54a-c4f49b09ee55">

Здесь подробно описан процесс обработки поступившего заказа приложением. Для успешного оформления заказа необходимо:
1) Указать валидный адрес доставки
2) Успешно оплатить заказ
3) Ресторан должен принять заказ

