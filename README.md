# YouTube Statistics Viewer

## Overview

The **YouTube Statistics Viewer** is a Python application built with Tkinter for a graphical user interface and MySQL for database management. This application allows users to explore YouTube video statistics from different regions (India, Canada, USA, and Great Britain) by applying various filters such as trending date, category, and numerical values like views, likes, dislikes, and comment counts.

## Features

- **Region Selection**: Users can select a region to view statistics for different countries.
- **Filter Options**: Users can filter data based on trending date, category, or numeric values.
- **Dynamic Data Display**: Results are displayed in a treeview format for easy analysis.
- **Error Handling**: The application includes validation and error handling for user inputs.

## Requirements

- Python 3.x
- Tkinter (for GUI)
- MySQL Connector (for database operations)
- A MySQL database named `youtube` with appropriate tables

## Setup

1. **Install Dependencies**

   Ensure you have the necessary Python packages installed. You can install them using pip:

   ```sh
   pip install mysql-connector-python
   ```

2. **Database Setup**

   Create a MySQL database named `youtube` and ensure the following tables are created with sample data:

   - `india`
   - `canada`
   - `united_states`
   - `great_britain`
   - `category` (for video categories)

   Adjust the MySQL connection parameters in the code if necessary.

3. **Run the Application**

   Save the provided code in a Python file, e.g., `youtube_statistics_viewer.py`, and run it:

   ```sh
   python youtube_statistics_viewer.py
   ```

   The application window will appear, allowing you to interact with the statistics viewer.

## Code Description

- **Imports**: The code imports necessary libraries including `tkinter`, `ttk`, `mysql.connector`, and `re`.
- **GUI Components**: The main window includes a region selection combobox and an explore button.
- **Filter Functions**: Various filter functions are implemented to handle user input and query the database.
- **Error Handling**: Functions for handling invalid inputs and displaying error messages.
- **Database Operations**: Functions connect to the MySQL database, execute SQL queries, and display results.
