<div align="center">
  <img alt="Rocket"
    src="https://hotmart.s3.amazonaws.com/product_contents/0569fee6-8c8f-4dee-a46d-80102ced177a/Header_Product_1920x450.jpg"
  />

</div>

<h2 align="center">
   Challenge 04: First NodeJS Project
</h2>

<h3 align="center">
  <img alt="NodeJS"
    src="https://arrayoutofindex.files.wordpress.com/2017/06/node.png" width="180px"/>
</h3>

<!-- <table align="center">
  <tr >
    <td>
      <img width="77px" alt="Sass logo" src="https://rawgit.com/sass/node-sass/master/media/logo.svg" />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
    </td>
    <td valign="center" >
      <span>Texte</span>
    </td>
  </tr>
</table> -->

<p align="center">

  <img alt="language version" src="https://img.shields.io/badge/Node-v_12.13.1-339933?logo=node.js">

  <img alt="language version" src="https://img.shields.io/badge/Yarn-v_1.22.4-2C8EBB?logo=Yarn">

  <img alt="GitHub language count" src="https://img.shields.io/github/languages/count/Fred-Reis/challenge_backEnd-04_GoStack-v2">

  <img alt="GitHub top language" src="https://img.shields.io/github/languages/top/Fred-Reis/challenge_backEnd-04_GoStack-v2">

  <img alt="GitHub repo size in bytes" src="https://img.shields.io/github/repo-size/Fred-Reis/challenge_backEnd-04_GoStack-v2">

  <a href="https://www.codacy.com/manual/Fred-Reis/challenge_backEnd-04_GoStack-v2?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Fred-Reis/challenge_backEnd-04_GoStack-v2&amp;utm_campaign=Badge_Grade">
    <img src="https://api.codacy.com/project/badge/Grade/3187a10038db4dd2bfc2b746d37ab925"/></a>

  <!-- <a href="https://app.netlify.com/sites/affectionate-mahavira-913f7b/deploys">
    <img src="https://api.netlify.com/api/v1/badges/0abef9c1-d6d2-4af3-a5e1-b24332614634/deploy-status"/></a> -->

</p>

<blockquote align="center">
  This project be a part of bootcamp:
    <a href="https://rocketseat.com.br/gostack">
      GoStack by RocketSeat
    </a>
</blockquote>

<hr/>

<h4 align="center">Links:</h4>

<p align="center">

  <a href="#-about-challenge">
    <img src="https://img.shields.io/badge/About_Challenge-a5a5a5"/>
  </a>&nbsp;&nbsp;
  <a href="#-architecture">
    <img src="https://img.shields.io/badge/Architecture-a5a5a5"/>
  </a>&nbsp;&nbsp;
  <a href="#-functionalities">
    <img src="https://img.shields.io/badge/Functionalities-a5a5a5"/>
  </a>&nbsp;&nbsp;
  <a href="-techs">
    <img src="https://img.shields.io/badge/Techs-a5a5a5"/>
  </a>&nbsp;&nbsp;
  <a href="#-tools">
    <img src="https://img.shields.io/badge/Tools-a5a5a5"/>
  </a>&nbsp;&nbsp;
  <a href="#-run-this-project">
    <img src="https://img.shields.io/badge/Run_this_project-a5a5a5"/>
  </a>&nbsp;&nbsp;
  <a href="#author-frederico-reis">
    <img src="https://img.shields.io/badge/Author-a5a5a5"/>
  </a>

</p>

## 💡 About Challenge:

In this challenge, construction began on the API that will serve as a front-end server and mobile application in the future.

Some concepts of SOLID and software architecture were applied.

## 📐 Architecture:

In this project, two routes were created divided into a project structure that
removes all liability from the route file, such as business rules and data validation. A structure with models, repositories and services was used to divide the tasks.

Folder's structure:

![estrutura](src/assets/readme/estrutura.png)

## 🔥 Functionalities:

- `POST /transactions`: This route receive `title`, `value` and `type` in the request body, being the `type` of transaction, which must be "income" for incoming (deposits) and "outcome" for outgoing (withdrawal). When registering a new transaction, it must be stored inside an object with the format as follows:

```js
{
  "id": "uuid",
  "title": "Salário",
  "value": 3000,
  "type": "income"
}
```

- `GET /transactions`: This route should return a list of all the transactions you have registered so far, together with the sum of the entries, withdrawals and total credit. This route must return an object with the following format:

```js
{
  "transactions": [
    {
      "id": "uuid",
      "title": "Salário",
      "value": 4000,
      "type": "income"
    },
    {
      "id": "uuid",
      "title": "Freela",
      "value": 2000,
      "type": "income"
    },
    {
      "id": "uuid",
      "title": "Pagamento da fatura",
      "value": 4000,
      "type": "outcome"
    },
    {
      "id": "uuid",
      "title": "Cadeira Gamer",
      "value": 1200,
      "type": "outcome"
    }
  ],
  "balance": {
    "income": 6000,
    "outcome": 5200,
    "total": 800
  }
}
```

## ⚙️ Techs:

- **NodeJS**;
- EsLint;
- Prettier;
- Express;
- Nodemon;
- Yarn;
- Jest;

## ⛏ Tools:

- [Insomnia](https://insomnia.rest/download/);
- [Notion](https://www.notion.so/?utm_source=google&utm_campaign=brand_alpha&utm_content=row&utm_term=notion&gclid=CjwKCAjw1cX0BRBmEiwAy9tKHs5ggnFG4dmfW38kOuGDTQS1-YjRGg01PuIriv8ftUuAUzeoU7QFFxoCAkIQAvD_BwE);

## 🏁 Run this project:

To run on the first time,
into your folder:

```bash
$ git clone https://github.com/Fred-Reis/challenge_backEnd-04_GoStack-v2
```

Into repo folder, to install `Node_Modules` run:

```bash
yarn
```

And to start the server:

```bash
yarn dev:server
```

> Recommend using [Insomnia](https://insomnia.rest/download/) to test routes

#### [For more details on the list of requirements and tests for this challenge.](https://github.com/Rocketseat/bootcamp-gostack-desafios/tree/master/desafio-fundamentos-nodejs)

😃 Now run this project and...
**BE HAPPY**.

<h4>
  😍 Thanks for you interest!
</h4>

<br/>

<h4 align="center">
  "Stay hungry stay foolish!"
</h4>

<br/>

---

<h3 align="center">
Author: <a alt="Fred-Reis" href="https://github.com/Fred-Reis">Frederico Reis</a>
</h3>

<p align="center">

  <a alt="Frederico Reis" href="https://www.linkedin.com/in/frederico-reis-dev/">
    <img src="https://img.shields.io/badge/LinkedIn-Frederico_Reis-0077B5?logo=linkedin"/></a>
  <a alt="Frederico Reis" href="https://github.com/Fred-Reis ">
  <img src="https://img.shields.io/badge/Fred_Reis-GitHub-000?logo=github"/></a>

</p>
