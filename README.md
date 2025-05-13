
# PlanQuote Pro - Insurance Quote Calculator

PlanQuote Pro is a web-based insurance quote calculator that helps users compute real-time insurance premiums based on age, coverage amount, and insurance type. It features risk analytics, quote history tracking, and interactive charts.

![Screenshot (112)](https://github.com/user-attachments/assets/a4854710-423f-4cd8-89ea-fdb17faa0ce1)
![Screenshot (113)](https://github.com/user-attachments/assets/52c45bcf-00c3-405f-960e-4358571d5a47)
![Screenshot (114)](https://github.com/user-attachments/assets/ae8c3197-c2b2-47a2-9cc6-ff255ff99571)
![Screenshot (115)](https://github.com/user-attachments/assets/026f8e46-3003-4645-9e88-3da83fdbacdb)
![Screenshot (116)](https://github.com/user-attachments/assets/7c74f20a-ba5c-48d4-a61f-d0d4285545af)

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

