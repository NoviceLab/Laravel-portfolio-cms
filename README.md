# Laravel Portfolio CMS

[![License](https://img.shields.io/github/license/NoviceLab/Laravel-portfolio-cms.svg)](LICENSE)
<!-- [![Build Status](https://travis-ci.com/NoviceLab/Laravel-portfolio-cms.svg?branch=main)](https://travis-ci.com/NoviceLab/Laravel-portfolio-cms) -->
[![Laravel Version](https://img.shields.io/badge/Laravel-10.x-red)](https://laravel.com)

**Laravel Portfolio CMS** is an open-source, flexible, and feature-rich content management system (CMS) tailored for developers, designers, and freelancers to easily create and manage their personal portfolios. Built with the Laravel framework, it provides a modern, user-friendly interface for customizing and displaying your work and professional profile.

## Key Features

- **Full CMS Functionality**: Manage your portfolio content, including projects, blog posts, and contact forms, through an intuitive admin panel.
- **Dynamic Portfolio**: Add, edit, and remove projects with detailed descriptions, images, and links to live demos or repositories.
- **Responsive Design**: Fully responsive and mobile-first design, ensuring seamless display across devices.
- **SEO-Optimized**: Pre-configured SEO-friendly URLs, meta tags, and social sharing capabilities.
- **Customizable Themes**: Easily switch and customize themes using Blade templates and SASS.
- **Blog Integration**: Publish articles, tutorials, or updates with the built-in blog feature.
- **Contact Form**: Integrated contact form with email notifications.
- **User Management**: Role-based access control for managing multiple users (Admin, Editor).
- **Built with Laravel 10.x**: Taking advantage of the latest Laravel features and security enhancements.

## Demo

Explore the live demo of the application:

- [Frontend Demo](https://portfolio.novicelab.tech)
- [Admin Panel Demo](https://portfolio.novicelab.tech/admin)  
  Username: `admin@novicelab.tech`  
  Password: `password123`

## Installation

### Prerequisites

Ensure your system meets the following requirements:

- PHP 8.1 or higher
- Composer
- MySQL or PostgreSQL
- Node.js & npm (for asset compilation)

### Step-by-Step Setup

1. **Clone the repository:**

    ```bash
    git clone https://github.com/NoviceLab/Laravel-portfolio-cms.git
    cd Laravel-portfolio-cms
    ```

2. **Install dependencies:**

    ```bash
    composer install
    npm install
    ```

3. **Create and configure `.env` file:**

    Copy the example environment file and adjust the database credentials and other settings:

    ```bash
    cp .env.example .env
    ```

    Edit the `.env` file with your preferred editor:

    ```bash
    DB_CONNECTION=mysql
    DB_HOST=127.0.0.1
    DB_PORT=3306
    DB_DATABASE=portfolio_cms
    DB_USERNAME=root
    DB_PASSWORD=secret
    ```

4. **Generate application key:**

    ```bash
    php artisan key:generate
    ```

5. **Run database migrations and seeders:**

    Set up the database structure and insert sample data:

    ```bash
    php artisan migrate --seed
    ```

6. **Compile assets:**

    Compile the frontend assets using Laravel Mix:

    ```bash
    npm run dev
    ```

7. **Serve the application:**

    Start the local development server:

    ```bash
    php artisan serve
    ```

    Access your portfolio CMS at `http://localhost:8000`.

## Features Overview

### Admin Panel

The admin panel allows you to:

- **Manage Portfolio Items**: Add or edit projects, upload images, write descriptions, and add tags.
- **Blog Management**: Create, edit, or delete blog posts with featured images and categories.
- **Contact Messages**: View and manage messages sent via the contact form.
- **User Management**: Control user roles, permissions, and passwords.

### Project Display

- **Dynamic Grid Layout**: Your portfolio projects are displayed in a dynamic, customizable grid with filterable categories.
- **Single Project View**: Each project includes a detailed view with images, descriptions, and links to live versions or GitHub repositories.

### Theme Customization

- Laravel Portfolio CMS supports multiple themes, and users can create their own by modifying Blade templates and stylesheets located in the `resources/views` directory.

## Contributing

We welcome contributions! To get started:

1. Fork the repository.
2. Create a new feature branch: `git checkout -b feature/my-new-feature`.
3. Commit your changes: `git commit -m 'Add some feature'`.
4. Push to the branch: `git push origin feature/my-new-feature`.
5. Submit a pull request.

Please read our [Contributing Guidelines](CONTRIBUTING.md) for more details.

## License

This project is open-sourced under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Support

For any issues or feature requests, feel free to create an issue in the GitHub repository or contact us at [novicelab.01@gmail.com](mailto:novicelab.01@gmail.com).

---

**Laravel Portfolio CMS** - Developed by [NoviceLab](https://novicelab.tech) | Powered by Laravel
