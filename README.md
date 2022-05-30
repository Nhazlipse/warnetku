# Warnetku

Warnetku is a web app for managing computer, operator, rental price and
rental transaction in an internet cafe(it's called warnet in my country).
This app is made to ease the work of internet cafe operators. For example,
determine the price to be paid by the customer.

![Web Status](https://img.shields.io/website.svg?url=https://warnetku.herokuapp.com&style=for-the-badge)

## ✨ Demo

Web url: https://warnetku.herokuapp.com  
You can use the account below for login access

| Username  | Password  | Role   |
| --------- | --------- | ------ |
| operator0 | operator0 | Owner  |
| operator1 | operator1 | Worker |

## 📑 Documentation

-   ### Computer

    Operator can see a list of all computers, along with their type and
    status. There are two types of computers: _Gaming_ and _Office_.
    Computer status can be _Used by ..._ or _Idle_. Operator with
    _Owner_ role can perform create, update and delete operations.

-   ### Price

    Operator can see a list of all rental prices, but can't perform add,
    update and delete operations. Only operator with _Owner_ role can
    do that thing.

-   ### Operator

    Only operator with _Owner_ role can access this page. This page
    serves to manage operator data (CRUD).

-   ### Transaction

    Operator cam add rental transaction at here. Operator can see other
    operator transaction but can't update and delete it. Each operator
    can only update and delete their own transaction. Except operator
    with _Owner_ role. The owner can update and delete other operator's
    transactions.

-   ### Report

    This page is about (simple)financial reports. It provides total
    income and transaction count for today, this month, and more.

## 📸 Screenshots

![Screenshot1](https://cdn.discordapp.com/attachments/946013429200723989/980702509024837732/Screenshot_from_2022-05-30_11-52-50.png)
![Screenshot2](https://cdn.discordapp.com/attachments/946013429200723989/980702509293240421/Screenshot_from_2022-05-30_11-53-32.png)
![Screenshot3](https://cdn.discordapp.com/attachments/946013429200723989/980702509536526346/Screenshot_from_2022-05-30_11-53-41.png)
![Screenshot4](https://cdn.discordapp.com/attachments/946013429200723989/980702509788180540/Screenshot_from_2022-05-30_11-53-47.png)
![Screenshot5](https://cdn.discordapp.com/attachments/946013429200723989/980702510018859048/Screenshot_from_2022-05-30_11-54-07.png)

## 💽 Database Structure

![Database](https://cdn.discordapp.com/attachments/946013429200723989/980702471963934780/drawSQL-export-2022-05-30_11_59.png)

## 🛠️ Development

```
# Clone the project
$ git clone https://github.com/BayuDC/warnetku.git
$ cd warnetku

# Install dependencies
$ composer install

# Create env file
$ cp .env.example .env

# Set all required variables
$ nano .env
# or using your favorite text editor

# Generate encryption key
$ php artisan key:generate

# Database migration
$ php aritsan migrate
# with seed
$ php artisan migrate --seed

$ Run dev server
$ php artisan serve
```

## 📝 Todo

-   Refactor, there are so many inefficient and repetitive code ✅
