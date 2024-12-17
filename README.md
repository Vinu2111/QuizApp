# QuizApp
Here's a clear and concise **GitHub project description** for your Quiz App:

---

# **Quiz App using Spring Boot** 🚀

This is a simple **Quiz Application** built using **Spring Boot** and **H2 Database**. The app allows users to start a new quiz session, answer multiple-choice questions, and track their performance. The backend APIs handle quiz management, random question retrieval, answer submission, and result calculation.

---

## **Features**

1. **Start New Quiz Session** 📋  
   - Users can start a fresh quiz session.

2. **Fetch Random Questions** 🎲  
   - A random multiple-choice question is fetched from the database for the user to answer.

3. **Submit Answers** ✅  
   - Users can submit their answers, and the system evaluates correctness.

4. **View Results and Stats** 📊  
   - Users can view the total number of questions attempted, along with counts of correct and incorrect submissions.

---

## **Tech Stack** 🛠️
- **Backend**: Java 18, Spring Boot
- **Database**: H2 (in-memory database)
- **ORM**: Spring Data JPA
- **Build Tool**: Maven
- **Testing**: JUnit

---

## **APIs**

| Method | Endpoint                          | Description                           |
|--------|----------------------------------|---------------------------------------|
| POST   | `/api/quiz/start`                | Start a new quiz session              |
| GET    | `/api/quiz/question/{sessionId}` | Fetch a random question               |
| POST   | `/api/quiz/submit`               | Submit an answer                      |
| GET    | `/api/quiz/stats/{sessionId}`    | Retrieve user quiz stats              |

---

## **How to Run Locally** 🚀

1. **Clone the repository**:  
   ```bash
   git clone https://github.com/yourusername/quiz-app.git
   cd quiz-app
   ```

2. **Build and run the project**:  
   Use Maven to build the project and run the Spring Boot application:  
   ```bash
   mvn spring-boot:run
   ```

3. **Access the APIs**:  
   The app will be available at:  
   ```
   http://localhost:8080
   ```

---

## **Database Configuration** 🗄️

The application uses an **H2 Database** for simplicity. The database schema and data are automatically initialized from the following files:

- **`schema.sql`**: Defines the database structure.
- **`data.sql`**: Seeds initial data (users and questions).

---

## **Assumptions** 📌

- A single user (`id: 1`) is pre-seeded in the database.
- Questions and answers are pre-seeded for demo purposes.
- The quiz supports multiple-choice questions with options **A, B, C, and D**.

---

## **Future Enhancements** 🚀
- Add support for multiple users.
- Implement frontend UI using React or Angular.
- Add a leaderboard to display top performers.
- Include timers for each question to increase difficulty.

---

## **Screenshots (Optional)** 📸
Add screenshots or API testing results here.

---

## **License** 📜
This project is licensed under the MIT License.

---

Feel free to modify this to fit your specific requirements. Let me know if you need further tweaks or additions! 🚀 
