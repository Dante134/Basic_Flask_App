# Basic_Flask_App

## Project Overview  

This project is a web application built using Flask that allows users to calculate the average of marks entered for three subjects: Maths, Science, and History. The application dynamically evaluates whether the user has passed or failed based on the average marks, providing an interactive and user-friendly experience. It is ideal for learners and developers looking to understand Flask routing, form handling, and template rendering.

---

## Project Steps  

### 1. Set Up the Environment  
   - **Tools Used**: Flask, Python  
   - **Goal**: Develop a simple web-based interface to input scores, calculate averages, and display results dynamically.  

### 2. Application Structure  
   - **`form.html`**: HTML template to capture user input for scores in three subjects.  
   - **`app.py`**: Flask application handling routes, form submission, and average score calculation logic.  
   - **`requirements.txt`**: File containing necessary Python dependencies.  

### 3. Application Features  
   - **Welcome and Index Pages**:  
     - Basic pages to navigate through the application.  
   - **Form Page**:  
     - Users input scores for Maths, Science, and History.  
     - Submit button to calculate the average marks.  
   - **Result Handling**:  
     - If the average score is 50 or above, the user is redirected to a success page displaying the average marks.  
     - If the average is below 50, the user is redirected to a failure page with the score.  

---

## Steps to Run the Project  

### 1. Clone the Repository  
```bash  
git clone <repo-url>  
```  

### 2. Install Dependencies  
```bash  
pip install -r requirements.txt  
```  

### 3. Run the Application  
```bash  
python app.py  
```  
Visit `http://127.0.0.1:5000` in your browser to interact with the application.  

---

## Project Files  

```plaintext  
|-- templates/                 # HTML templates for the application  
|    |-- form.html             # User input form template  
|-- app.py                     # Main Flask application  
|-- requirements.txt           # Python dependencies  
```  

---

## Code Explanation  

### 1. `app.py` (Flask Routing)  
   - **Route: `/`**: Displays a welcome message.  
   - **Route: `/index`**: A placeholder index page.  
   - **Route: `/form`**: Renders the form for inputting subject marks and calculates average on submission.  
   - **Route: `/success/<score>`**: Displays a success message with the average score.  
   - **Route: `/fail/<score>`**: Displays a failure message with the average score.  

### 2. `form.html` (User Interface)  
   - A simple form to input scores for three subjects.  
   - Displays the calculated average dynamically on submission.

---

## Requirements  

- **Python 3.8+**  
- **Flask**  

### `requirements.txt`:  
```plaintext  
Flask==2.1.2  
```  

---

## Future Enhancements  

- **Validation**: Add checks for invalid inputs (e.g., negative scores).  
- **Styling**: Enhance the form and result pages with CSS.  
- **Result Insights**: Include additional details such as total marks and grade distribution.  
- **Deployment**: Host the application on a cloud platform like Heroku or AWS.  

---

## License  

This project is licensed under the MIT License.  

---  

## Acknowledgments  

- Flask documentation for routing and form handling.  
- Community contributions for Flask-based beginner projects.  
