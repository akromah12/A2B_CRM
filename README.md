# AI-Powered CRM for SMEs (A2B CRM)

## Project Overview
A2B CRM is an AI-driven Customer Relationship Management (CRM) solution designed for Small and Medium Enterprises (SMEs). It integrates artificial intelligence features such as sentiment analysis, chatbots, and predictive analytics to enhance customer engagement and automate business workflows.

## Features
- AI-powered chatbot for automated customer interactions
- Sentiment analysis for customer feedback and communication
- Predictive analytics for lead scoring and customer retention
- Interactive dashboards for customer insights
- Secure authentication and role-based access control

## Requirements
To set up the project locally, ensure you have the following installed:

1. **XAMPP (PHP & MySQL)** – [Download Here](https://www.apachefriends.org/download.html)
2. **Composer (PHP Dependency Manager)** – [Download Here](https://getcomposer.org/download/)
3. **Node.js & npm** – [Download Here](https://nodejs.org/)
4. **Git (Version Control)** – [Download Here](https://git-scm.com/downloads)

## Installation Guide

### 1. Clone the Repository

### 2. Install Dependencies
```sh
composer install
```

### 3. Set Up Environment Variables
Copy the `.env.example` file and rename it to `.env`. 
Then, generate the application key:
```sh
php artisan key:generate
```
Link the storage directory

```
php artisan storage:link
```

### 4. Configure the Database
Create a MySQL database matching the name set in `.env`. Then, run migrations:
```sh
php artisan migrate --seed
```

### 5. Start the Development Server
```sh
php artisan serve
```

### 6. Compile Frontend Assets
```sh
npm run dev
```

## API Integration
This project integrates AI services via external APIs (e.g., OpenAI). To configure API access, add your API keys in the `.env` file:
```sh
AI_API_KEY=your_api_key_here

```

## Basic Commands
| Command | Description |
|---------|-------------|
| `php artisan migrate` | Run database migrations |
| `php artisan db:seed` | Seed the database with test data |
| `php artisan serve` | Start the Laravel development server |
| `npm run dev` | Compile frontend assets |
| `php artisan test` | Run application tests |

## Contributing
1. Create a feature branch: `git checkout -b feature-branch-name`.
2. Commit your changes: `git commit -m 'Add new feature'`.
. Push to the branch: `git push origin feature-branch-name`.
5. Open a pull request.


