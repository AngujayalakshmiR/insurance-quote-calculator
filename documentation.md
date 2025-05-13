# PlanQuote Pro - Insurance Quote Calculator
## Technical Documentation

### 1. Introduction
PlanQuote Pro is a web-based insurance quote calculator that helps users calculate insurance premiums based on various factors. The application provides real-time premium calculations, risk analysis, and historical data tracking.

### 2. System Architecture
- **Frontend**: HTML, CSS, JavaScript, Bootstrap 5
- **Backend**: Spring Boot (Java)
- **Database**: MySQL
- **Charts**: Chart.js
- **Alerts**: SweetAlert2

### 3. Features

#### 3.1 Premium Calculator
- Real-time premium calculation
- Multiple insurance types support (Life, Health, Auto)
- Dynamic risk assessment
- Interactive charts and visualizations

#### 3.2 Risk Analytics
- Age-based risk assessment
- Coverage amount risk analysis
- Insurance type risk factors
- Visual representation through charts

#### 3.3 Quote History
- Complete quote history tracking
- Delete functionality
- Formatted display of all quotes
- Responsive table design

### 4. Premium Calculation Logic

#### 4.1 Base Premium
```java
basePremium = coverageAmount * 0.05
```

#### 4.2 Risk Factors

##### Age Factors:
- < 25 years: 1.5x
- 25-34 years: 1.2x
- 35-44 years: 1.0x
- 45-54 years: 1.1x
- 55-64 years: 1.3x
- 65+ years: 2.0x

##### Coverage Amount Factors:
- ≤ 5L: 1.0x
- 5L-10L: 1.2x
- 10L-20L: 1.4x
- 20L-50L: 1.6x
- > 50L: 2.0x

##### Insurance Type Factors:
- Life Insurance: 1.2x
- Health Insurance: 1.5x
- Auto Insurance: 1.8x

#### 4.3 Final Premium Calculation
```java
finalPremium = basePremium * ageFactor * coverageFactor * typeFactor
```

### 5. User Interface

#### 5.1 Main Page (Calculator)
- Input form for quote calculation
- Premium analysis chart
- Risk ratio analysis chart
- Navigation menu

#### 5.2 History Page
- Tabular display of all quotes
- Delete functionality
- Formatted currency display
- Responsive design

#### 5.3 Risk Analytics Page
- Age-based risk assessment chart
- Insurance type risk analysis
- Risk summary statistics

### 6. Database Schema

#### 6.1 InsuranceQuote Table
```sql
CREATE TABLE insurance_quote (
    id BIGINT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(255),
    age INT,
    insurance_type VARCHAR(50),
    coverage_amount DOUBLE,
    premium DOUBLE,
    calculation_date DATETIME
);
```

### 7. API Endpoints

#### 7.1 GET Endpoints
- `/`: Main calculator page
- `/history`: Quote history page
- `/risk-analytics`: Risk analytics page

#### 7.2 POST Endpoints
- `/calculate`: Calculate new insurance quote

#### 7.3 DELETE Endpoints
- `/delete-quote/{id}`: Delete a specific quote

### 8. Installation and Setup

#### 8.1 Prerequisites
- Java JDK 8 or higher
- Maven
- MySQL
- XAMPP (for local development)

#### 8.2 Setup Steps
1. Clone the repository
2. Configure database connection in `application.properties`
3. Run `mvn spring-boot:run`
4. Access the application at `http://localhost:8080`

### 9. Security Features
- Input validation
- SQL injection prevention
- XSS protection
- CSRF protection

### 10. Error Handling
- Form validation errors
- Database connection errors
- Calculation errors
- User-friendly error messages

### 11. Future Enhancements
1. User authentication and authorization
2. PDF quote generation
3. Email functionality
4. Advanced analytics
5. Mobile application
6. Payment gateway integration

### 12. Maintenance
- Regular database backups
- Log monitoring
- Performance optimization
- Security updates

### 13. Support
For technical support or queries, contact:
- Developer: Angu Jayalakshmi R
- Email: [Your Email]
- Version: 1.0.0

### 14. License
© 2025 PlanQuote Pro. All rights reserved.

---

*This documentation is maintained by the development team and should be updated with any significant changes to the application.* 