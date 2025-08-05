# <span align="center" style="color: #3498db;" > TDLFAPI</span>
![2MGXgbaBdCjhJIYuq_ab7WgicC41IHQuUkFwLuEkhi4hJngsISB0bA](https://github.com/user-attachments/assets/3188eb48-9348-4f3c-a441-b54d338c6fb1)


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
 - [Пример запроса](./Examples/Request/API/V1/ProductIFZ.json)

 Доступные реквизиты необходимо добавить в обмен.

## Цены
### Отправить цены на товар

```http
  POST /api/v1/PriceIFZ
```
- [Пример запроса](./Examples/Request/API/V1/PriceIFZ.json)


## Остатки
### Отправить остатки товаров

```http
  POST /api/v1/StockIFZ
```
- [Пример запроса](./Examples/Request/API/V1/StockIFZ.json)


## Отгрузка
### Отправить список отгрузок

```http
  POST /api/v1/PostShipmentIFZ
```











## Секция титл
## 2
## Acknowledgements

 - [Awesome Readme Templates](https://awesomeopensource.com/project/elangosundar/awesome-README-templates)
 - [Awesome README](https://github.com/matiassingers/awesome-readme)
 - [How to write a Good readme](https://bulldogjob.com/news/449-how-to-write-a-good-readme-for-your-github-project)


## API Reference

#### Get all items

```http
  GET /api/items
```

| Parameter | Type     | Description                |
| :-------- | :------- | :-|
| `api_key` | `string` | **Required**. Your API key |

#### Get item

```http
  GET /api/items/${id}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`      | `string` | **Required**. Id of item to fetch |

#### add(num1, num2)

Takes two numbers and returns the sum.


## Badges

Add badges from somewhere like: [shields.io](https://shields.io/)

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)
[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)


## Demo

Insert gif or link to demo


## Features

- Light/dark mode toggle
- Live previews
- Fullscreen mode
- Cross platform

## Color Reference

| Color             | Hex                                                                |
| ----------------- | ------------------------------------------------------------------ |
| Example Color | ![#0a192f](https://via.placeholder.com/10/0a192f?text=+) #0a192f |
| Example Color | ![#f8f8f8](https://via.placeholder.com/10/f8f8f8?text=+) #f8f8f8 |
| Example Color | ![#00b48a](https://via.placeholder.com/10/00b48a?text=+) #00b48a |
| Example Color | ![#00d1a0](https://via.placeholder.com/10/00b48a?text=+) #00d1a0 |


## Deployment

To deploy this project run

```bash
  npm run deploy
```


## Documentation

[Documentation](https://linktodocumentation)


## Contributing

Contributions are always welcome!

See `contributing.md` for ways to get started.

Please adhere to this project's `code of conduct`.


# Hi, I'm Katherine! 👋


## 🚀 About Me
I'm a full stack developer...


## Other Common Github Profile Sections
👩‍💻 I'm currently working on...

🧠 I'm currently learning...

👯‍♀️ I'm looking to collaborate on...

🤔 I'm looking for help with...

💬 Ask me about...

📫 How to reach me...

😄 Pronouns...

⚡️ Fun fact...


## Installation

Install my-project with npm

```bash
  npm install my-project
  cd my-project
```
    
## Lessons Learned

What did you learn while building this project? What challenges did you face and how did you overcome them?


![Logo](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/th5xamgrr6se0x5ro4g6.png)

![Logo](https://cdn1.ozonusercontent.com/s3/product-service-meta-media/8e367f05-6c44-4dde-8032-b48c0d85d417.jpg)
## Optimizations

What optimizations did you make in your code? E.g. refactors, performance improvements, accessibility


## Roadmap

- Additional browser support

- Add more integrations


## Screenshots

![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here)


## Run Locally

Clone the project

```bash
  git clone https://link-to-project
```

Go to the project directory

```bash
  cd my-project
```

Install dependencies

```bash
  npm install
```

Start the server

```bash
  npm run start
```


## Tech Stack

**Client:** React, Redux, TailwindCSS

**Server:** Node, Express


## Usage/Examples

```javascript
import Component from 'my-project'

function App() {
  return <Component />
}
```


## Running Tests

To run tests, run the following command

```bash
  npm run test
```


## Used By

This project is used by the following companies:

- Company 1
- Company 2
