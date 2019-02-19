# Week 3 Notes

This week we are going to be building our first full application! In Week 1 we learned about routing and request types, in Week 2 we learned about creating HTML pages. We are now going to build our own servers and deploy websites locally! This is one of the most exciting lessons to build.

## [Laravel](https://laravel.com/)

We are going to be using something called a "framework" to deploy our own applications. Laravel is a framework written in the programming language of `PHP`. It's a full stack framework, which means it encompasses both the front-end (HTML, what you see) and the back-end (PHP, how it works). Don't worry if you don't know PHP - **everything we are learning is going to be language and framework agnostic, meaning you can easily pick up any other framework**.

Laravel is a Model-View-Controller (MVC) framework, meaning it revolves around the idea of using these components to share information. We'll get into exactly what this means at a later time. For now, let's get things set up!

## Deploying Laravel on Mac

### Installing Homebrew

To get started, you need to install Homebrew on your Mac. Homebrew is a package management system for your computer. You can download it from their [website here](https://brew.sh/), or run this command in your terminal: 

```bash
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

```

### Installing Composer

Composer is a PHP package manager. To install it you will need to follow the [instructions here.](https://getcomposer.org/doc/00-intro.md) Or run these commands:

```bash
php composer-setup.php --install-dir=bin --filename=composer
```

Now run, this will make it available globally:

```bash
mv composer.phar /usr/local/bin/composer
```

To check that things are working, type `composer` in your terminal in any directory: 

![composer](/src/composer.png)

### Installer PHP in Homebrew

Now run this command:

```bash
brew install php
```

This will install PHP on your local machine through Homebrew. You can run `brew services list` to see all of the installed Homebrew packages.

### Laravel Installer

Run this command to install the Laravel Installer: 

```bash
composer global require laravel/installer
```

Now install Valet (this will boot a local server):

```bash
composer global require laravel/valet
```

Now install it:

```bash
valet install
```

To check that Valet is installed, run: `ping foobar.test`. You should see a list of web responses like this:

![valet-test](/src/valet-test.png)

### Installing First Laravel Project

Now we will install our first project. To do this, we want to create a new directory within your Home Directory that is called `Code`. Inside the Code folder we will have all of our Laravel Projects. Now run:

```bash
laravel new blog
```

And you can now access this site by going to: http://blog.test in your web browser.

## Deploying Laravel on Windows

## Laravel File Structure Basics

