**Проект e-commerce**
<br>Необходимо проанализировать совершенные покупки (запрос от продакт-менеджера)
<br>Файлы:
<br>**olist_customers_datase.csv** – таблица с уникальными идентификаторами пользователей
<br>o	customer_id – позаказный идентификатор пользователя
<br>o	customer_unique_id –  уникальный идентификатор пользователя  (аналог номера паспорта)
<br>o	customer_zip_code_prefix –  почтовый индекс пользователя
<br>o	customer_city –  город доставки пользователя
<br>o	customer_state –  штат доставки пользователя
<br>**olist_orders_dataset.csv** –  таблица заказов
<br>o	order_id –  уникальный идентификатор заказа (номер чека)
<br>o	customer_id –  позаказный идентификатор пользователя
<br>o	order_status –  статус заказа
<br>o	order_purchase_timestamp –  время создания заказа
<br>o	order_approved_at –  время подтверждения оплаты заказа
<br>o	order_delivered_carrier_date –  время передачи заказа в логистическую службу
<br>o	order_delivered_customer_date –  время доставки заказа
<br>o	order_estimated_delivery_date –  обещанная дата доставки
<br>**olist_order_items_dataset.csv** –  товарные позиции, входящие в заказы
<br>o	order_id –  уникальный идентификатор заказа (номер чека)
<br>o	order_item_id –  идентификатор товара внутри одного заказа
<br>o	product_id –  ид товара (аналог штрихкода)
<br>o	seller_id – ид производителя товара
<br>o	shipping_limit_date –  максимальная дата доставки продавцом для передачи заказа партнеру по логистике
<br>o	price –  цена за единицу товара
<br>o	freight_value –  вес товара
<br>Уникальные статусы заказов в таблице olist_orders_dataset:
<br>-	created –  создан
<br>-	approved –  подтверждён
<br>-	invoiced –  выставлен счёт
<br>-	processing –  в процессе сборки заказа
<br>-	shipped –  отгружен со склада
<br>-	delivered –  доставлен пользователю
<br>-	unavailable –  недоступен
<br>-	canceled –  отменён
