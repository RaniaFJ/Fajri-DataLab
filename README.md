# Fajri DataLab  

**Fajri DataLab** is a web application built with Django that offers a comprehensive platform for **data analysis** and **visualization**. Users can securely upload CSV files, explore datasets, generate statistical summaries, and create interactive data visualizations.  

---

## Features  

### CSV File Handling  
- Upload and store CSV files for analysis.  
- Export processed datasets back to CSV for offline use.  

### Data Analysis  
- Generate statistical insights (mean, median, standard deviation, etc.).  
- Encode categorical variables (Label Encoding and One-Hot Encoding).  

### Interactive Data Visualization  
- Create dynamic charts using **Plotly**, including:  
  - Histograms  
  - Scatter plots  
  - Bar charts  
  - Line plots  
  - Pie charts  
  - Box plots  

### Data Exploration  
- View specific rows or columns in a dataset.  
- Filter and explore data interactively.  

### Secure User Authentication  
- Secure login system to manage file uploads and access data.  

---

## Prerequisites  

To run this project locally, ensure the following are installed:  
- Python 3.x  
- Django  
- Pandas  
- Plotly  
- Other dependencies listed in `requirements.txt`  

---

## Installation  

### 1. Clone the Repository  
```bash  
git clone https://github.com/your-username/data-analysis-project.git  
cd data-analysis-project  
```  

### 2. Install Dependencies  
```bash  
pip install -r requirements.txt  
```  

### 3. Configure the Database  
```bash  
python manage.py migrate  
```  

### 4. Run the Development Server  
```bash  
python manage.py runserver  
```  
Access the application at [http://127.0.0.1:8000/](http://127.0.0.1:8000/).  

---

## Project Structure  
```  
data_analysis_project/  
├── data_analysis/                 # Django app for core functionalities  
│   ├── migrations/                # Database migrations  
│   ├── static/                    # Static assets (CSS, JS, images)  
│   ├── templates/                 # HTML templates for views  
│   │   ├── show_data.html         # Display data and plots  
│   │   └── upload_csv.html        # CSV upload form  
│   ├── forms.py                   # CSV file upload form  
│   ├── models.py                  # Models for handling uploaded data  
│   ├── views.py                   # Logic for data analysis and visualization  
│   ├── urls.py                    # App-specific routes  
├── media/                         # Uploaded files  
├── manage.py                      # Django management script  
├── requirements.txt               # Python dependencies  
└── README.md                      # Project documentation  
```  

---

## Usage  

### 1. Upload a CSV File  
- Navigate to the **Upload CSV** page.  
- Upload your CSV file.  

### 2. Analyze the Data  
- View statistical summaries of your dataset.  
- Generate and interact with visualizations.  

### 3. Explore and Export  
- Filter rows/columns for specific insights.  
- Export datasets to a CSV format.  

---

## Security  
- **Authentication**: Secure login functionality protects file uploads and data access.  
- **Data Encoding**: Automatically encodes categorical variables for analysis.  

---

## Future Enhancements  
- Advanced data filtering based on user-defined conditions.  
- Additional visualization options (e.g., heatmaps, tree maps).  
- Automated data cleaning tools for handling missing or duplicate values.  
- Machine learning integration for predictive analytics.  

---

## Dependencies  
The application uses the following libraries:  
- **Django**: Web framework.  
- **Pandas**: Data manipulation and analysis.  
- **Plotly**: Interactive visualizations.  
