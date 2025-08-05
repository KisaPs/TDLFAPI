# <span align="center" style="color: #3498db;text-align:center" > TDLFAPI</span>

<img width="148" height="142" alt="600008557279b2" src="https://github.com/user-attachments/assets/05c2a677-ce15-4d80-a85b-52e6f57c410f" />


##### URL будет задан позже, проводятся работы
  
## Служебные
### Проверка доступности

```http
  GET /api/v1/ping
```

## Заказ
### Получить новые заказы

```http
  GET /api/v1/InvoiceIFZ
```
 - При отстутствии заказов вернуть пустой массив. 
 - Назначение может быть пустое. 
 - Назначения необходимо группировать, это раздельные Заказы Клиентов.

 [Пример ответа](./Examples/Response/API/V1/GetInvoiceIFZ.json)

### Подтвердить прием заказов

```http
  POST /api/v1/InvoiceIFZ
```
 - [Пример запроса](./Examples/Request/API/V1/PostInvoiceIFZ.json)
 - [Пример ответа](./Examples/Response/API/V1/PostInvoiceIFZ.json)

  "status":  "success", "partial" или "error".  
  После установки резерва, обновить остатки.

## Товары
### Отправить номенклатуру

```http
  POST /api/v1/ProductIFZ
```
 - [Пример запроса](./Examples/Request/API/V1/PostProductIFZ.json)

 Доступные реквизиты необходимо добавить в обмен.

## Цены
### Отправить цены на товар

```http
  POST /api/v1/PriceIFZ
```
- [Пример запроса](./Examples/Request/API/V1/PostPriceIFZ.json)


## Остатки
### Отправить остатки товаров

```http
  POST /api/v1/StockIFZ
```
- [Пример запроса](./Examples/Request/API/V1/PostStockIFZ.json)


## Отгрузка
### Отправить список отгрузок

```http
  POST /api/v1/PostShipmentIFZ
```

### Обновить список отгрузок

```http
  PUT /api/v1/PostShipmentIFZ
```

## Сборка
### Отправить список отгрузок

```http
  POST /api/v1/OrderIFZ
```

### Обновить список отгрузок

```http
  PUT /api/v1/OrderIFZ
```




| Метод | Название                     | Путь API                         | Якорь                     |
|-------|------------------------------|----------------------------------|---------------------------|
| GET   | [Получить новые заказы](#получить-заказы) | `/api/v1/InvoiceIFZ`          | `#получить-заказы`        |
| POST  | [Подтвердить прием заказов](#подтвердить-заказы) | `/api/v1/InvoiceIFZ`          | `#подтвердить-заказы`     |
| POST  | [Отправить номенклатуру](#отправить-номенклатуру) | `/api/v1/ProductIFZ`         | `#отправить-номенклатуру` |
| POST  | [Отправить цены](#отправить-цены) | `/api/v1/PriceIFZ`            | `#отправить-цены`         |
| POST  | [Отправить остатки](#отправить-остатки) | `/api/v1/StockIFZ`            | `#отправить-остатки`      |
| POST  | [Отправить отгрузки](#отправить-отгрузки) | `/api/v1/PostShipmentIFZ`     | `#отправить-отгрузки`     |
| PUT   | [Обновить отгрузки](#обновить-отгрузки) | `/api/v1/PostShipmentIFZ`     | `#обновить-отгрузки`      |
| POST  | [Отправить сборки](#отправить-сборки) | `/api/v1/OrderIFZ`            | `#отправить-сборки`       |
| PUT   | [Обновить сборки](#обновить-сборки) | `/api/v1/OrderIFZ`            | `#обновить-сборки`        |

## Детализация методов

### <a id="получить-заказы"></a> Получить новые заказы
```http
GET /api/v1/InvoiceIFZ


# Безопасность
| Parameter | Type     | Description                |
| :-------- | :------- | :-----|
| `api_key` | `string` | **Required**. Your API key |

