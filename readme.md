![IronHack_Logo](https://user-images.githubusercontent.com/92721547/180665853-e52e3369-9973-4c1e-8d88-1ecef1eb8e9e.png)

# Lab | Deploying a Data Science Project with Django

In this lab, you will create a web application using Django to deploy a machine learning model. You can use the Iris dataset classification model (same as used for Flask) or train and save another model of your choice.

## Prerequisites

- Python 3.7+ installed
- Basic knowledge of Python and machine learning
- Virtual environment setup knowledge

## Lab Instructions

### Step 1: Project Setup
1. Create a new project directory and navigate to it
2. Create and activate a virtual environment
3. Install required packages: `django`, `scikit-learn`, `pandas`, `numpy`, `joblib`
4. Create a new Django project called `ml_project`
5. Create a Django app called `predictor`
6. Add your app to `INSTALLED_APPS` in settings.py

### Step 2: Prepare Your Model

Choose one of the following options:

**Option A: Use Iris Classification Model (Recommended)**
- Use the same Iris dataset classification model from the Flask lesson

**Option B: Build Your Own Model**
1. Choose your own dataset and machine learning problem
2. Train a classification or regression model of your choice
3. Save your trained model as a `.pkl` file in your project root

### Step 3: Create Views
1. Create views in `predictor/views.py`:
   - A `home` view to display the input form
   - A `predict` view to handle form submission and return predictions
2. Load your saved model in the views file
3. Handle user input validation and error cases

### Step 4: Configure URLs
1. Create `predictor/urls.py` with URL patterns for your views
2. Include your app URLs in the main `ml_project/urls.py`

### Step 5: Create Templates
1. Create a `templates/predictor/` directory structure
2. Create the following HTML templates:
   - `base.html` - Base template with navigation and Bootstrap CSS
   - `home.html` - Form for user input (extends base template)
   - `result.html` - Display prediction results (extends base template)

### Step 6: Test Your Application
1. Run Django migrations: `python manage.py migrate`
2. Start the development server: `python manage.py runserver`
3. Test your application in the browser
4. Verify that:
   - Input form displays correctly
   - Model predictions work as expected
   - Error handling works for invalid inputs
   - Results are displayed properly

## Deliverables

Your completed Django application should include:
- Working web interface for model predictions
- Proper error handling for invalid inputs
- Clean, responsive design using Bootstrap
- Proper project structure with templates and static files
- Screenshot of your Django Web application running on Local Host.

## Submission

- Upon completion, add your deliverables to git. 
- Then commit git and push your branch to the remote.
- Make a pull request and paste the PR link in the submission field in the Student Portal.

<br>

**Good luck!**