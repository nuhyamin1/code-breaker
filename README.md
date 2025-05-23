# CallGraphAnalyzer - Python Code Structure and Call Visualizer

This simple web application helps you visualize the structure of your Python code and understand its call relationships. Upload a `.py` file, and it will generate an interactive force-graph showing classes and functions. Clicking on a function or method node not only displays its code but also highlights where it's called from within the analyzed file.

## Screenshot

![Application Screenshot](./images/screenshot.png)
![Application Screenshot](./images/screenshot2.png)

## Features

*   **File Upload:** Accepts Python (`.py`) files.
*   **Structure Visualization:** Displays a hierarchical tree view of classes, methods, and top-level functions using D3.js.
*   **Call Relationship Visualization:** Interactively see which functions or methods call a selected function/method. Clicking a node highlights incoming calls, making it easy to trace execution flow.
*   **Code Snippet Display:** Click on any class or function node in the tree to view its source code directly on the page.
*   **Simple Web Interface:** Built with Flask for the backend and basic HTML/CSS/JavaScript for the frontend.

## Setup

To get this running on your local machine, follow these steps:

1.  **Prerequisites:** Make sure you have Python 3.x and pip installed.
2.  **Clone the Repository:**
    ```bash
    git clone https://github.com/nuhyamin1/CallGraphAnalyzer.git
    ```
3.  **Navigate to Directory:** Open your terminal or command prompt and change into the newly cloned `CallGraphAnalyzer` directory.
4.  **Virtual Environment (Recommended):**
    ```bash
    python -m venv venv
    # On Windows
    .\venv\Scripts\activate
    # On macOS/Linux
    source venv/bin/activate
    ```
5.  **Install Dependencies:** The only external library needed is Flask.
    ```bash
    pip install Flask
    ```

## Running the Application

1.  Make sure you are in the project directory in your terminal and your virtual environment (if used) is activated.
2.  Run the Flask development server:
    ```bash
    python app.py
    ```
3.  Flask will start the server, usually at `http://127.0.0.1:5000`. Open this URL in your web browser.

## How to Use

1.  Once the application is running in your browser, you'll see a file input field.
2.  Click **"Choose File"** and select a Python (`.py`) file from your computer.
3.  Click the **"Analyze File"** button.
4.  An interactive tree diagram representing the code structure will appear.
5.  Click on any class or function node in the diagram.
6.  The corresponding source code for that node will be displayed in the box below the diagram. If you click on a function or method, arrows will also appear on the diagram showing which other functions/methods call the selected one.
