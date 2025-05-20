# Open Weather API Ajax Search Widget

**Widget by Rjay Ibina | Full-stack Developer (PHP / WordPress) Code Documentation**

## Code Documentation

This project is built as a child theme for the Storefront theme. Below are the key implementations and code documentation for the project:

### 1. Child Theme Setup

- A child theme for the Storefront theme was created to manage all custom modifications.

### 2. Custom Post Type: Cities

- A custom post type called **“Cities”** was created using hooks.
  - Code Location: `functions.php` (Lines 14-25)

### 3. Meta Boxes for Latitude and Longitude

- A meta box with custom fields **“latitude”** and **“longitude”** was added for entering the respective coordinates of the city.
  - Code Location: `functions.php` (Lines 40-78)

### 4. Custom Taxonomy: Countries

- A custom taxonomy titled **“Countries”** was created and attached to the **“Cities”** post type.
  - Code Location: `functions.php` (Lines 28-37)

### 5. Cities Widget

- A widget was developed to display city names along with their current temperatures fetched from an external API (e.g., OpenWeatherMap).
  - File Created: `widget-cities.php`

### 6. Custom Template for Countries and Cities Table

- A custom template was created to display a table listing countries, cities, and temperatures.
  - File Created: `template-cities.php`
  - Data is retrieved using a database query with the global variable `$wpdb`.
  - A search field for cities was added above the table using WP Ajax, along with custom action hooks before and after the table.
  - Code Location: `functions.php` (Lines 81-152)

## App Demonstration

=======
# openweather-ajax-search-wordpress
A custom WordPress widget that uses AJAX and the OpenWeather API to display real-time weather data based on user input. Built with PHP, JavaScript, and jQuery for dynamic and responsive weather search functionality.