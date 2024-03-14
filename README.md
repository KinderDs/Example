<div align='center'>
  # <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="30px"/>
</div>

### В ходе проекта проведём анализ совершенных покупок и ответим на следующие вопросы:

---

*  Сколько пользователей совершили покупку только один раз?
*  Сколько заказов в месяц в среднем не доставляется по разным причинам?
*  В какой день недели каждый товар чаще всего покупается?
*  Сколько у каждого из пользователей в среднем покупок в неделю (по месяцам)?

*  Проведём когортный анализ пользователей и определим когорту с самым высоким retention на 3й месяц в период с января по декабрь.
*  Построим RFM-сегментацию пользователей.

---

<details>
  <summary><b> 🛠 &nbsp;&nbsp;Используемые данные:&nbsp;</b></summary>
  <br/> 
<div>
<details>
  <summary><b>&nbsp;&nbsp;olist_customers_datase.csv — таблица с уникальными идентификаторами пользователей&nbsp;</b></summary>
  
* customer_id — позаказный идентификатор пользователя

* customer_unique_id —  уникальный идентификатор пользователя  (аналог номера паспорта)

*  customer_zip_code_prefix —  почтовый индекс пользователя

*  customer_city —  город доставки пользователя

*  customer_state —  штат доставки пользователя


</details>


<details>
  <summary><b>&nbsp;&nbsp;olist_orders_dataset.csv —  таблица заказов&nbsp;</b></summary>
  
*  order_id —  уникальный идентификатор заказа (номер чека)

*  customer_id —  позаказный идентификатор пользователя
  
*  order_status —  статус заказа
  
*  order_purchase_timestamp —  время создания заказа
  
*  order_approved_at —  время подтверждения оплаты заказа
  
*  order_delivered_carrier_date —  время передачи заказа в логистическую службу
  
*  order_delivered_customer_date —  время доставки заказа
  
*  order_estimated_delivery_date —  обещанная дата доставки

</details>

<details>
  <summary><b>&nbsp;&nbsp;olist_order_items_dataset.csv —  товарные позиции, входящие в заказы&nbsp;</b></summary>
  
*  order_id —  уникальный идентификатор заказа (номер чека)
  
*  order_item_id —  идентификатор товара внутри одного заказа
   
*  product_id —  ид товара (аналог штрихкода)
   
*  seller_id — ид производителя товара
   
*  shipping_limit_date —  максимальная дата доставки продавцом для передачи заказа партнеру по логистике
   
*  price —  цена за единицу товара
  
*  freight_value —  вес товара
</details>
</div>
</details>
