# PlanQuote Pro - Insurance Quote Calculator

PlanQuote Pro is a web-based insurance quote calculator that helps users compute real-time insurance premiums based on age, coverage amount, and insurance type. It features risk analytics, quote history tracking, and interactive charts.

## 🚀 Features

- Real-time premium calculation
- Support for Life, Health, and Auto Insurance
- Risk analysis with visual charts
- Quote history with delete option
- Responsive UI with Bootstrap 5
 
## 🛠 Tech Stack

- **Frontend:** HTML, CSS, JavaScript, Bootstrap 5
- **Backend:** Spring Boot (Java)
- **Database:** MySQL
- **Charts:** Chart.js
- **Alerts:** SweetAlert2

## 📦 Installation

1. Clone the repository  
   `git clone https://github.com/yourusername/planquote-pro.git`

2. Configure MySQL database in `application.properties`

3. Run the application  
   `mvn spring-boot:run`

4. Open in browser  
   `http://localhost:8080`

## 📌 API Endpoints

- `GET /` - Calculator Page  
- `GET /history` - View Quotes  
- `GET /risk-analytics` - Risk Charts  
- `POST /calculate` - Calculate Premium  
- `DELETE /delete-quote/{id}` - Delete Quote

## 📧 Support

**Developer:** Angu Jayalakshmi R  
**Email:** angujayalakshmi2005@gmail.com

