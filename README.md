# eInvoice

eInvoice is a web-based invoicing application built with PHP. This project allows users to generate and manage invoices with features such as JSON/XML generation and API key testing. **Note: This application is for development and testing purposes only and is not intended for production use.**

• USE ONLY GENERATE JSON/XML, TEST YOUR API KEYS, NOT MEANT FOR PRODUCTION.  
![image](https://github.com/user-attachments/assets/52c46caf-6d0c-4cb3-9206-70fd7f7a8ed3)


## Table of Contents

- [Requirements](#requirements)
- [Installation](#installation)
- [Configuration](#configuration)
- [Running the Application](#running-the-application)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [LHDN References](#lhdn-references)
- [Acknowledgment](#acknowledgment)

## Requirements

Before you begin, ensure you have met the following requirements:

- Windows operating system.
- XAMPP with PHP 8.1 or higher installed.
- Composer installed for PHP dependency management.

## Installation

### Step 1: Install XAMPP

1. Download and install XAMPP from the [official website](https://www.apachefriends.org/).
2. Ensure that PHP 8.1 or higher is included in your XAMPP installation.

### Step 2: Verify PHP Installation

After installing XAMPP, verify the PHP installation:

1. Open the Command Prompt or PowerShell.
2. Navigate to the PHP directory within XAMPP:
   ```bash
   cd C:\xampp\php
   ```
3. Check the PHP version by running:
   ```bash
   php -v
   ```
   You should see the PHP version displayed.

### Step 3: Install Composer

1. Download Composer from the [official website](https://getcomposer.org/).
2. Run the installer and follow the prompts to install Composer.
3. Verify the Composer installation:
   ```bash
   composer -V
   ```

### Step 4: Clone the Repository

1. Fork the original repository to your GitHub account.
2. Clone your forked repository:
   ```bash
   git clone https://github.com/yourusername/eInvoice.git
   ```
3. Navigate to the project directory:
   ```bash
   cd eInvoice
   ```

### Step 5: Enable Required PHP Extensions

1. Open the `php.ini` file located in the XAMPP installation directory:
   ```bash
   C:\xampp\php\php.ini
   ```
2. Enable the following extensions by removing the semicolons (`;`) at the beginning of their lines:
   ```ini
   extension=intl
   extension=xsl
   extension=sodium
   extension=zip
   ```
3. Save the `php.ini` file.
4. Restart Apache using the XAMPP Control Panel.

### Step 6: Install Project Dependencies

1. Install the necessary PHP dependencies using Composer:
   ```bash
   composer install
   ```
2. If you encounter any issues with the lock file, you can update the dependencies:
   ```bash
   composer update
   ```

## Configuration

### Step 1: Set Up Environment Variables

1. In the project directory, rename the `.env.example` file to `.env`:
   ```bash
   mv .env.example .env
   ```
2. Generate an application key:
   ```bash
   php artisan key:generate
   ```

## Running the Application

1. Start the development server:
   ```bash
   php artisan serve
   ```
2. Open your web browser and navigate to `http://localhost:8000` to access the application.

## Usage

The eInvoice application allows you to:

- Generate JSON/XML representations of invoices.
- Test your API keys.

**Note:** This application is intended for development and testing purposes only and is not suitable for production use.

## Contributing

Contributions are welcome! Please fork the repository, make your changes, and submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## LHDN References

- [Login as Taxpayer System](https://sdk.myinvois.hasil.gov.my/api/07-login-as-taxpayer-system/)
- [Get Document Types](https://sdk.myinvois.hasil.gov.my/api/03-get-document-types/)

## Acknowledgment

This repository is a fork of the original eInvoice project by [irvine48]. I have made some changes and improvements to better suit my needs. All credit for the original work goes to the original author.
