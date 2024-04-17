<div align='center'>
<h1>
  Когортный и RFM анализы!
  <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="30px"/>
</h1>
</div>
<div align='center'>
   <img src="https://img.shields.io/badge/Python-%23AFEEEE?style=for-the-badge&logo=Python&logoColor=yellow"/>
   <img src="https://img.shields.io/badge/pandas-%23AFEEEE?style=for-the-badge&logo=pandas&logoColor=white"/>
   <img src="https://img.shields.io/badge/Seaborn-%23AFEEEE?style=for-the-badge&logo=Seaborn"/>
   <img src="https://img.shields.io/badge/matplotlib-%23AFEEEE?style=for-the-badge&logo=matplotlib&logoColor=white"/>
   <img src="https://img.shields.io/badge/numpy%20-%23AFEEEE?style=for-the-badge&logo=numpy%20&logoColor=white"/>
</div>

## В ходе анализа данных совершенных покупок:
* ### Определил:
  * ### Сколько пользователей совершили покупку только один раз.
  * ### Сколько заказов в месяц в среднем не доставляется по разным причинам.
  * ### В какой день недели каждый товар чаще всего покупается.
  * ### Сколько у каждого из пользователей в среднем покупок в неделю (по месяцам).
* ### Провёл когортный анализ пользователей.
* ### Построил RFM-сегментацию пользователей.
---
## В результате:
* выявил, что наибольший процент товаров не доставляется в назначенный срок, следовательно, необходимо пересмотреть сроки доставки или оптимизировать работу логистической службы.
* Стоит обратить внимание, что основа продаж приходится на будние дни, а пик продаж некоторых товаров во вторник.
* Проведя когортный анализ, определил, что менее 1% пользователей совершают повторные покупки. Следует, что бизнесу необходимо придумать новую стратегию удержания клиентов.
* На основе RFM анализа определил процент ценных пользователей и тех, которые находятся в зоне риска. Маркетологам необходимо придумать подход к «потенциальным клиентам» и к тем, которых необходимо «реанимировать», чтобы перестать терять 15% клиентов в год.
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
