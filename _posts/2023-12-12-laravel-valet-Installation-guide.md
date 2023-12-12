---
title: "Comprehensive Guide to Installing Laravel and Laravel Valet on MacOS"
author: ariffin
date: 2023-12-12 10:59:00 +0800
categories: [Blogging, Laravel]
tags: [Laravel]
---

# Introduction
Embarking on your Laravel journey on MacOS? This detailed guide will walk you through installing Composer, Laravel, and Laravel Valet. Get ready to set up a robust PHP development environment on your MacOS machine! 🚀

## Prerequisites
Before starting, ensure that you have:
- MacOS running on your computer
- Homebrew installed (Visit [Homebrew](https://brew.sh/) for installation instructions)

## Step 1: Installing PHP and Composer with Homebrew
PHP and Composer are essential for Laravel. Install them using Homebrew:

### Install PHP
```bash
brew install php
```

### Install Composer
```bash
brew install composer
```

## Step 2: Adding Composer to Your PATH
To ensure global access to Composer, add it to your `$PATH` in your `~/.bash_profile` or `~/.zshrc` file:
```bash
export PATH="$HOME/.composer/vendor/bin:$PATH"
```
Then, reload your profile:
```bash
source ~/.bash_profile
# Or, if you're using Zsh
source ~/.zshrc
```

## Step 3: Installing Laravel
With Composer installed, you can now install Laravel:
```bash
composer global require laravel/installer
```
This command installs Laravel globally, enabling you to create new Laravel projects easily.

## Step 4: Installing Laravel Valet
Laravel Valet is a lightweight development environment for MacOS. To install it:

### Install Valet with Composer
```bash
composer global require laravel/valet
```

### Run the Valet installation command
```bash
valet install
```
After installation, Valet will start the necessary background services, like Nginx.

## Step 5: Configuring and Using Laravel Valet
- **Park Directories:** Run `valet park` in a directory to serve all projects within.
- **Link Individual Projects:** Use `valet link project-name` in a project directory to serve it as `http://project-name.test`.

## Step 6: Running Your Laravel Project
To run your Laravel project:
```bash
valet open
```
Or access it at `http://project-name.test` in your browser. 🌐

## Conclusion
You're now equipped with Laravel and Laravel Valet on your MacOS. This setup is ideal for a smooth and efficient development process. Dive into Laravel and create amazing applications! 🚀👨‍💻👩‍💻

## Additional Resources
- [Laravel Documentation](https://laravel.com/docs)
- [Laravel Valet Documentation](https://laravel.com/docs/valet)

---

Explore these tools and refer to the official documentation for advanced configurations and troubleshooting. Happy coding! 🎈👩‍💻👨‍💻