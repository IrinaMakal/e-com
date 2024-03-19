**Проект e-commerce**
Необходимо проанализировать совершенные покупки (запрос от продакт-менеджера)
Файлы:
**olist_customers_datase.csv** – таблица с уникальными идентификаторами пользователей
o	customer_id – позаказный идентификатор пользователя
o	customer_unique_id –  уникальный идентификатор пользователя  (аналог номера паспорта)
o	customer_zip_code_prefix –  почтовый индекс пользователя
o	customer_city –  город доставки пользователя
o	customer_state –  штат доставки пользователя
**olist_orders_dataset.csv** –  таблица заказов
o	order_id –  уникальный идентификатор заказа (номер чека)
o	customer_id –  позаказный идентификатор пользователя
o	order_status –  статус заказа
o	order_purchase_timestamp –  время создания заказа
o	order_approved_at –  время подтверждения оплаты заказа
o	order_delivered_carrier_date –  время передачи заказа в логистическую службу
o	order_delivered_customer_date –  время доставки заказа
o	order_estimated_delivery_date –  обещанная дата доставки
**olist_order_items_dataset.csv** –  товарные позиции, входящие в заказы
o	order_id –  уникальный идентификатор заказа (номер чека)
o	order_item_id –  идентификатор товара внутри одного заказа
o	product_id –  ид товара (аналог штрихкода)
o	seller_id – ид производителя товара
o	shipping_limit_date –  максимальная дата доставки продавцом для передачи заказа партнеру по логистике
o	price –  цена за единицу товара
o	freight_value –  вес товара
Уникальные статусы заказов в таблице olist_orders_dataset:
-	created –  создан
-	approved –  подтверждён
-	invoiced –  выставлен счёт
-	processing –  в процессе сборки заказа
-	shipped –  отгружен со склада
-	delivered –  доставлен пользователю
-	unavailable –  недоступен
-	canceled –  отменён
