# 🗳️ Voting Survey Application

The **Voting Survey** is a full-stack web application that allows users to register, vote, and view survey results in a secure and user-friendly way. The application is built using **Spring Boot** for the backend and **React** for the frontend, with support for image upload and user profile display.

---

## 📌 Features

- ✅ Voter Registration with Image Upload (Base64 encoded)
- ✅ User Authentication
- ✅ Voting Functionality (One-time voting)
- ✅ Constituency-based candidate selection
- ✅ Admin Dashboard (Manage voters and results)
- ✅ Responsive UI built with React
- ✅ RESTful APIs with Spring Boot

---

## 🛠️ Tech Stack

### Backend
- Java 17
- Spring Boot
- Spring MVC
- Spring Data JPA (Hibernate)
- MySQL Database
- Lombok

### Frontend
- React.js
- Axios (for API requests)
- React Hooks
- CSS (Custom styling)

---

## 📁 Project Structure

### Backend (Spring Boot)
```
src/
├── main/
│   ├── java/com/jspider/votingsurvey/
│   │   ├── controller/
│   │   ├── dto/
│   │   ├── entity/
│   │   ├── repository/
│   │   ├── service/
│   │   └── VotingSurveyApplication.java
│   └── resources/
│       ├── application.properties
│       └── schema.sql / data.sql
```

### Frontend (React)
```
voting-survey-frontend/
├── public/
├── src/
│   ├── components/
│   ├── pages/
│   ├── services/
│   └── App.js
```

---

## ⚙️ Setup Instructions

### Backend (Spring Boot)

1. Clone the repo:
   ```bash
   git clone https://github.com/your-username/voting-survey.git
   cd voting-survey
   ```

2. Update `application.properties` with your MySQL credentials:
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/voting_db
   spring.datasource.username=root
   spring.datasource.password=your_password
   ```

3. Run the Spring Boot application:
   ```bash
   mvn spring-boot:run
   ```

---

### Frontend (React)

1. Navigate to the frontend folder:
   ```bash
   cd voting-survey-frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm start
   ```

---

## 📷 Image Upload

- Users can upload a profile picture during registration.
- Image is converted to a Base64 string in the frontend and sent via JSON to the backend.
- Image is stored as a Base64-encoded string in the database.
- Displayed using:  
  ```html
  <img src={`data:image/jpeg;base64,${userImg}`} />
  ```

---

## 🚀 Future Improvements

- JWT Authentication
- Role-based access control (Admin/User)
- Pagination and filtering
- Chart-based survey result display
- Image storage using AWS S3 or local file system

---

## 👨‍💻 Author

**Aamir Shahab**  
Java Full Stack Developer  
Lucknow, India  
🔗 [LinkedIn](https://www.linkedin.com/in/aamirs582001/)

---

## 📜 License

This project is licensed under the MIT License.

