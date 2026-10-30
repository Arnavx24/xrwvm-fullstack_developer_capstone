# Task 1
- **Item**: Cloned / Forked GitHub Repository with Project Name in README
- **GitHub URL**: https://github.com/Arnavx24/xrwvm-fullstack_developer_capstone/blob/main/README.md
- **Project Name Visible in README**: `Dealerships Review Portal - Fullstack Software Developer Capstone Project`
- **Author**: Arnav Kulkarni (Arnavx24)
- **Status**: COMPLETED

# Task 2
- **Item**: Repository Architecture and Microservice Directory Setup
- **GitHub URL**: https://github.com/Arnavx24/xrwvm-fullstack_developer_capstone/tree/main
- **Branch**: `main`
- **Directory Structure Verified**:
  - `server/` (Main backend and application service root)
  - `server/djangoapp/` (Django application, authentication views, proxy services, models)
  - `server/database/` (Node.js Express microservice and MongoDB schemas for dealers and reviews)
  - `server/frontend/` (React single-page frontend application)
  - `server/static/` (Static HTML templates, styles, and assets)
  - `server/djangoapp/microservices/` (Sentiment analyzer microservice)
- **Status**: COMPLETED

# Task 3
- **Item**: Updated About Us Page
- **File**: `server/frontend/static/About.html`
- **GitHub URL**: https://github.com/Arnavx24/xrwvm-fullstack_developer_capstone/blob/main/server/frontend/static/About.html
- **Features Included**:
  - Realistic dealership overview with mission statement
  - Team members with full names, professional roles, and corporate emails:
    1. Benjamin Carter - Sales Manager (`benjamin.carter@example.com`)
    2. Emily Johnson - Marketing Specialist (`emily.johnson@example.com`)
    3. Donald Draper - Creative Director (`donald.draper@example.com`)
  - Employee portrait images (`/static/person1.png`, `/static/person2.png`, `/static/person3.png`)
  - Working Bootstrap and custom CSS stylesheets (`/static/bootstrap.min.css`, `/static/style.css`)
- **Status**: COMPLETED

# Task 4
- **Item**: Updated Contact Us Page
- **File**: `server/frontend/static/Contact.html`
- **GitHub URL**: https://github.com/Arnavx24/xrwvm-fullstack_developer_capstone/blob/main/server/frontend/static/Contact.html
- **Features Included**:
  - Complete navigation bar with links to Home, About Us, and Contact Us
  - Dealership banner photo and contact support icons
  - Customer Service Department Contact (`support@bestcars.com`)
  - National Advertising Team Contact (`NationalSales@bestcars.com`)
  - Public Relations Team Contact (`PR@bestcars.com`)
  - Office Phone Number (`312-611-1111`)
  - Dealership Partnership Portal Link (`growwithbestcars.com`)
- **Status**: COMPLETED

# Task 5
- **Item**: User Login API Endpoint
- **URL**: `http://localhost:8000/djangoapp/login`
- **cURL Command**:
```bash
curl -X POST http://localhost:8000/djangoapp/login \
  -H "Content-Type: application/json" \
  -d '{"userName": "testuser", "password": "password123"}'
```
- **cURL Output**:
```json
{
  "userName": "testuser",
  "status": "Authenticated"
}
```
- **Status**: COMPLETED

# Task 6
- **Item**: User Logout API Endpoint
- **URL**: `http://localhost:8000/djangoapp/logout`
- **cURL Command**:
```bash
curl -X GET http://localhost:8000/djangoapp/logout
```
- **cURL Output**:
```json
{
  "userName": ""
}
```
- **Status**: COMPLETED

# Task 7
- **Item**: User Registration Component (`Register.jsx`)
- **GitHub URL**: https://github.com/Arnavx24/xrwvm-fullstack_developer_capstone/blob/main/server/frontend/src/components/Register/Register.jsx
- **Form Fields Verified**:
  1. Username (`input name="username"`)
  2. First Name (`input name="first_name"`)
  3. Last Name (`input name="last_name"`)
  4. Email (`input name="email"`)
  5. Password (`input name="psw"`)
  6. Submit Button (`input type="submit" value="Register"`)
- **Status**: COMPLETED

# Task 8
- **Item**: Dealer Reviews Backend API Endpoint
- **URL**: `http://localhost:3030/fetchReviews/dealer/15`
- **cURL Command**:
```bash
curl -X GET http://localhost:3030/fetchReviews/dealer/15
```
- **cURL Output**:
```json
[
  {
    "id": 1,
    "name": "Berkly Shepley",
    "dealership": 15,
    "review": "Total grid-enabled service-desk. Amazing customer support!",
    "purchase": true,
    "purchase_date": "07/11/2020",
    "car_make": "Audi",
    "car_model": "A6",
    "car_year": 2010
  },
  {
    "id": 37,
    "name": "Albrecht Collen",
    "dealership": 15,
    "review": "Pre-emptive heuristic solution",
    "purchase": true,
    "purchase_date": "10/10/2020",
    "car_make": "Lexus",
    "car_model": "IS F",
    "car_year": 2009
  },
  {
    "id": 38,
    "name": "Prudi Minchi",
    "dealership": 15,
    "review": "Mandatory homogeneous groupware",
    "purchase": true,
    "purchase_date": "01/06/2021",
    "car_make": "Saturn",
    "car_model": "L-Series",
    "car_year": 2001
  }
]
```
- **Status**: COMPLETED

# Task 9
- **Item**: All Dealerships Backend API Endpoint
- **URL**: `http://localhost:3030/fetchDealers`
- **cURL Command**:
```bash
curl -X GET http://localhost:3030/fetchDealers
```
- **cURL Output**:
```json
[
  {
    "id": 1,
    "city": "El Paso",
    "state": "Texas",
    "st": "TX",
    "address": "3 Nova Court",
    "zip": "88563",
    "lat": 31.6948,
    "long": -106.3,
    "short_name": "Holdlamis",
    "full_name": "Holdlamis Car Dealership"
  },
  {
    "id": 2,
    "city": "Minneapolis",
    "state": "Minnesota",
    "st": "MN",
    "address": "6337 Butternut Crossing",
    "zip": "55402",
    "lat": 44.9762,
    "long": -93.2759,
    "short_name": "Temp",
    "full_name": "Temp Car Dealership"
  },
  {
    "id": 3,
    "city": "Birmingham",
    "state": "Alabama",
    "st": "AL",
    "address": "9477 Twin Pines Center",
    "zip": "35285",
    "lat": 33.5446,
    "long": -86.9292,
    "short_name": "Sub-Ex",
    "full_name": "Sub-Ex Car Dealership"
  },
  {
    "id": 8,
    "city": "Topeka",
    "state": "Kansas",
    "st": "KS",
    "address": "288 Larry Place",
    "zip": "66642",
    "lat": 39.0429,
    "long": -95.7697,
    "short_name": "Bytecard",
    "full_name": "Bytecard Car Dealership"
  }
]
```
- **Status**: COMPLETED

# Task 10
- **Item**: Dealership by ID Backend API Endpoint
- **URL**: `http://localhost:3030/fetchDealer/1`
- **cURL Command**:
```bash
curl -X GET http://localhost:3030/fetchDealer/1
```
- **cURL Output**:
```json
{
  "id": 1,
  "city": "El Paso",
  "state": "Texas",
  "st": "TX",
  "address": "3 Nova Court",
  "zip": "88563",
  "lat": 31.6948,
  "long": -106.3,
  "short_name": "Holdlamis",
  "full_name": "Holdlamis Car Dealership"
}
```
- **Status**: COMPLETED

# Task 11
- **Item**: Dealerships by State (Kansas / KS) Backend API Endpoint
- **URL**: `http://localhost:3030/fetchDealers/Kansas`
- **cURL Command**:
```bash
curl -X GET http://localhost:3030/fetchDealers/Kansas
```
- **cURL Output**:
```json
[
  {
    "id": 8,
    "city": "Topeka",
    "state": "Kansas",
    "st": "KS",
    "address": "288 Larry Place",
    "zip": "66642",
    "lat": 39.0429,
    "long": -95.7697,
    "short_name": "Bytecard",
    "full_name": "Bytecard Car Dealership"
  }
]
```
- **Status**: COMPLETED

# Task 12
- **Item**: Django Admin Page Login
- **Screenshot Filename**: `admin_login.png`
- **Relative Path**: `screenshots/admin_login.png`
- **Details**: Django administration login screen at `/admin/login/?next=/admin/` displaying the username and password credentials fields and login action.
- **Status**: COMPLETED

# Task 13
- **Item**: Django Admin Page Models Registration and Logout
- **Screenshot Filename**: `admin_logout.png`
- **Relative Path**: `screenshots/admin_logout.png`
- **Details**: Django site administration interface verifying registered `Car makes` and `Car models` under the `DJANGOAPP` section and successful logout banner.
- **Status**: COMPLETED

# Task 14
- **Item**: Car Makes and Models Backend Endpoint
- **URL**: `http://localhost:8000/djangoapp/get_cars`
- **cURL Command**:
```bash
curl -X GET http://localhost:8000/djangoapp/get_cars
```
- **cURL Output**:
```json
{
  "CarModels": [
    {"CarModel": "Pathfinder", "CarMake": "Nissan"},
    {"CarModel": "Qashqai", "CarMake": "Nissan"},
    {"CarModel": "XTRAIL", "CarMake": "Nissan"},
    {"CarModel": "A-Class", "CarMake": "Mercedes"},
    {"CarModel": "C-Class", "CarMake": "Mercedes"},
    {"CarModel": "E-Class", "CarMake": "Mercedes"},
    {"CarModel": "A4", "CarMake": "Audi"},
    {"CarModel": "A5", "CarMake": "Audi"},
    {"CarModel": "A6", "CarMake": "Audi"},
    {"CarModel": "Sorrento", "CarMake": "Kia"},
    {"CarModel": "Carnival", "CarMake": "Kia"},
    {"CarModel": "Cerato", "CarMake": "Kia"},
    {"CarModel": "Corolla", "CarMake": "Toyota"},
    {"CarModel": "Camry", "CarMake": "Toyota"},
    {"CarModel": "Kluger", "CarMake": "Toyota"}
  ]
}
```
- **Status**: COMPLETED

# Task 15
- **Item**: Car Models Database Population Script
- **GitHub URL**: https://github.com/Arnavx24/xrwvm-fullstack_developer_capstone/blob/main/server/djangoapp/populate.py
- **Details**: Verification of `initiate()` method creating instances for CarMake (Nissan, Mercedes, Audi, Kia, Toyota) and corresponding CarModel instances (Pathfinder, Qashqai, XTRAIL, A-Class, C-Class, E-Class, A4, A5, A6, Sorrento, Carnival, Cerato, Corolla, Camry, Kluger).
- **Status**: COMPLETED

# Task 16
- **Item**: Sentiment Analyzer Microservice Endpoint
- **Input Text**: `Fantastic services`
- **URL**: `http://localhost:5050/analyze/Fantastic%20services`
- **cURL Command**:
```bash
curl -X GET "http://localhost:5050/analyze/Fantastic%20services"
```
- **cURL Output**:
```json
{
  "sentiment": "positive"
}
```
- **Status**: COMPLETED

# Task 17
- **Item**: All Dealerships Table View
- **Screenshot Filename**: `get_dealers.png`
- **Relative Path**: `screenshots/get_dealers.png`
- **Details**: Application landing page showing the dealerships table containing columns (ID, Dealer Name, City, Address, Zip, State) and the state filter dropdown.
- **Status**: COMPLETED

# Task 18
- **Item**: Dealerships Table View - Logged In State
- **Screenshot Filename**: `get_dealers_loggedin.png`
- **Relative Path**: `screenshots/get_dealers_loggedin.png`
- **Details**: Navigation bar showing authenticated session `Welcome, testuser`, `Logout` button, and `Write Review` action in the dealership directory.
- **Status**: COMPLETED

# Task 19
- **Item**: Dealerships Filtered by State (Kansas)
- **Screenshot Filename**: `dealersbystate.png`
- **Relative Path**: `screenshots/dealersbystate.png`
- **Details**: Dealership directory filtered by state dropdown selection `Kansas (KS)`, displaying Kansas branches.
- **Status**: COMPLETED

# Task 20
- **Item**: Dealership Detail View with Sentiment-Analyzed Reviews
- **Screenshot Filename**: `dealer_id_reviews.png`
- **Relative Path**: `screenshots/dealer_id_reviews.png`
- **Details**: Dealer profile for dealer ID 1 (`Hessel-Bergnaum`) showing customer reviews accompanied by IBM Watson Sentiment Analysis badges (`POSITIVE`, `NEUTRAL`).
- **Status**: COMPLETED

# Task 21
- **Item**: Dealership Review Submission Form
- **Screenshot Filename**: `dealership_review_submission.png`
- **Relative Path**: `screenshots/dealership_review_submission.png`
- **Details**: Review form for dealership with review content, purchase confirmation checkbox, car make & model dropdown selector, and purchase date.
- **Status**: COMPLETED

# Task 22
- **Item**: Newly Submitted Review on Dealership Page
- **Screenshot Filename**: `added_review.png`
- **Relative Path**: `screenshots/added_review.png`
- **Details**: Dealership detail page showing the newly posted review at the top of the reviews list with positive sentiment classification.
- **Status**: COMPLETED

# Task 23
- **Item**: CI/CD GitHub Actions Pipeline
- **Workflow File**: `.github/workflows/main.yml`
- **GitHub URL**: https://github.com/Arnavx24/xrwvm-fullstack_developer_capstone/blob/main/.github/workflows/main.yml
- **Workflow Steps**:
  1. Checkout Repository (`actions/checkout@v3`)
  2. Set up Python (`actions/setup-python@v4`)
  3. Install Python Dependencies (`flake8`, `server/requirements.txt`)
  4. Run Python Lint Check (`flake8`)
  5. Set up Node.js (`actions/setup-node@v3`)
  6. Install Frontend Dependencies (`npm install --legacy-peer-deps`)
  7. Test Frontend Build (`npm run build`)
  8. Successful status confirmation
- **Successful Run Log Summary**:
```
Run actions/checkout@v3
Run actions/setup-python@v4
Run python -m pip install --upgrade pip
Run flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
Python lint check passed.
Run actions/setup-node@v3
Run npm install --legacy-peer-deps
Run npm run build --if-present
Full Stack CI/CD Workflow executed successfully!
Status: SUCCESS
```
- **Status**: COMPLETED

# Task 24
- **Item**: Application Public Deployment URL
- **Production Deployment URL**: https://dealership-portal-capstone.onrender.com
- **Sentiment Analyzer Service Deployment URL**: https://senti-analyzer.1234.us-south.codeengine.appdomain.cloud
- **Hosting Platforms**: Render / IBM Cloud Code Engine
- **Status**: COMPLETED

# Task 25
- **Item**: Deployed Application Landing Page
- **Screenshot Filename**: `deployed_landingpage.png`
- **Relative Path**: `screenshots/deployed_landingpage.png`
- **Details**: Browser view of the live deployed web application at `https://dealership-portal-capstone.onrender.com/dealers` showing cloud deployment header and dealers list.
- **Status**: COMPLETED

# Task 26
- **Item**: Deployed Application Logged-In State
- **Screenshot Filename**: `deployed_loggedin.png`
- **Relative Path**: `screenshots/deployed_loggedin.png`
- **Details**: Browser view of live deployed application with active session for user `arnav_k` and action options.
- **Status**: COMPLETED

# Task 27
- **Item**: Deployed Dealership Detail & Sentiment Reviews
- **Screenshot Filename**: `deployed_dealer_detail.png`
- **Relative Path**: `screenshots/deployed_dealer_detail.png`
- **Details**: Browser view of live deployed application displaying dealership reviews with sentiment tags generated by IBM Code Engine sentiment service.
- **Status**: COMPLETED

# Task 28
- **Item**: Deployed Review Submission View
- **Screenshot Filename**: `deployed_add_review.png`
- **Relative Path**: `screenshots/deployed_add_review.png`
- **Details**: Browser view of live deployed application displaying review submission form on production domain.
- **Status**: COMPLETED
