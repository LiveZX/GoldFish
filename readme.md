<div align="center">
<img src="https://i.imgur.com/DcZUxIi.gif" alt="Goldfish logo" />
</div>

## Work In Progress!
Goldfish v2 is currently a **Work In Progress**, unexpected error and bugs may & will occur, use it on your own responsibility.

*The project is only a side project of mine, and I only work on it when I have the time & motiviation to do so. There's still **a lot** to do before this version is production ready. As soon as I feel like the CMS is stable enough, I'll make a public release of the CMS - You're of course allowed to use the CMS at any time before that too.*

## What is Goldfish CMS?
GoldFish is a Content Management System (CMS) made for Habbo retros. It is built to allow you to offer a beatiful and managable website for you and your users.

## Who made Goldfish CMS
Goldfish CMS was originally made by [Laynester](https://github.com/Laynester/GoldFish)

## What is Goldfish v2
Goldfish v2 is a maintained, updated & refactored version original Goldfish CMS, with permission from Laynester. I (Object) decided to start the Goldfish v2 project, to offer a bigger variety of CMS' to select from, when setting up your hotel.

## What does Goldfish CMS offer?
Goldfish CMS offers a modern and industry approved backend, featuring the PHP framework Laravel and support for the most recent PHP version (PHP 8.1).

Besides the above it also offers a ton of features, most which you'd normally expect from a retro CMS, and even comes with its own theme system, that allows you to build your own themes, may it be with TailwindCSS, Bootstrap, Bulma, Vanilla CSS - you name it!

**What technologies is being used?**
- Laravel 8.x (Latest as of January 2022)
  [Laravel docs](https://laravel.com/docs/8.x).
- Bootstrap 5
  [Bootstrap docs](https://getbootstrap.com/docs/5.0/getting-started/introduction/).

## Setup guide
To install Goldfish CMS you'll need to do the following:
- PHP 8.1 or above [PHP Downloads](https://www.php.net/downloads.php)
- Composer v2 [Composer Download](https://getcomposer.org/download/)
- NPM (LTS) [Node Download](https://nodejs.org/en/download/)
- An Arcturus Morningstar database [Database repository](https://git.krews.org/morningstar/arcturus-morningstar-base-database)

After all of the above has been installed you've to do the following:
- Open CMD and navigate into the path you want the CMS to be located at, and run the commands listed below

#### Windows
```
git clone https://github.com/ObjectRetros/GoldFish.git
cd GoldFish
copy .env.example .env
composer install
composer require doctrine/dbal
npm install && npm run dev
php artisan key:generate
php artisan migrate --seed
```
#### Linux
```
git clone https://github.com/ObjectRetros/GoldFish.git
cd GoldFish
For Linux: cp .env.example .env
composer install
composer require doctrine/dbal
npm install && npm run dev
php artisan key:generate
php artisan migrate --seed
```

If all of the above steps has been done correctly / successfully, you should be prompted with an easy to follow installation process, once that has been finished, your CMS should be ready to use!
