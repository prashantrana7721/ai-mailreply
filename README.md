# AI-Email-Reply-Assistant

An intelligent email reply assistant that automatically generates context-aware email responses using Google's Gemini AI . This tool is a browser-based application with a Chrome extension for seamless integration with your email client .

---

## Live Demo & Screenshots

Here is a glimpse of the AI-Email-Reply-Assistant in action , generating a professional reply for a production incident escalation email .

#### Application In Action

<img width="1054" height="737" alt="Screenshot 2025-08-27 at 6 18 30 PM" src="https://github.com/user-attachments/assets/04eb0626-fa32-4189-98ad-458cb509551b" />

#### Request Response Test

<img width="1036" height="746" alt="Screenshot 2025-08-27 at 6 59 58 PM" src="https://github.com/user-attachments/assets/8ceef7ac-f607-4f95-9803-3ea4bb06a8b5" />


<br/>

---

## Core Features

*   **AI-Powered Replies:** Generates intelligent and relevant email replies based on the original email's content .
*   **Contextual Awareness:** The assistant analyzes the original email to create a reply that is both accurate and contextually appropriate .
*   **Tone Selection:** Users can select the tone of the reply ( e.g., Professional , Casual , Friendly ) .
*   **Seamless Integration:** A Chrome extension provides a smooth user experience, integrating directly with your email client's interface .
*   **Robust Backend:** Built with Java and Spring Boot for a scalable and reliable service .

---

## Tech Stack

This Project Is Built With A Modern And Robust Set Of Technologies :

*   **Back-End:** Java 17 , Spring Boot , Spring Web , Maven
*   **AI Service:** Google Gemini Pro API
*   **Front-End:** React + Vite , HTML , CSS , JavaScript
*   **Testing & Tools:** Postman , Git , IntelliJ IDEA , VS Code

---

## Getting Started

To Get A Local Copy Up And Running , Follow These Simple Steps :

### Prerequisites

*   **Java Development Kit (JDK) 17** or newer.
*   **Apache Maven**
*   **Node.js & npm**
*   **Git** for version control.
*   A **Google Gemini API Key**. You can get one from [Google AI Studio](https://aistudio.google.com/app/apikey).

### Installation & Configuration

1.  **Clone The Repository :**
    ```sh
    git clone https://github.com/your_username/ai-mailreply.git
    cd ai-mailreply
    ```

2.  **Configure Your API Key :**
    This Project Uses A `.env` File To Manage Secret Keys Securely . Create A New File Named `.env` In The Root Directory Of The Project .

3.  **Add Your API Key To The `.env` File :**
    ```
    GEMINI_API_KEY=AIzaSyYOUR_REAL_API_KEY_HERE
    ```

4.  **Important:** Add The `.env` File To Your `.gitignore` To Ensure You Don't Commit Your Secret Key To Version Control .
    ```gitignore
    # Ignore Local Environment Variables
    .env
    ```

### Running The Application

1.  **Run The Spring Boot Back-End:**
    Navigate to the backend directory .

    ```sh
    cd email-writer-sb
    chmod +x mvnw
    ./mvnw spring-boot:run
    ```
    The Server Will Start On `localhost:8080` .

2.  **Run The React Front-End:**
    Open a new terminal and navigate to the frontend directory .

    ```sh
    cd email-writer-ext
    npm install
    npm run dev
    ```
    The frontend will be available at `localhost:5173` .

---

## API Endpoint

The Primary API End-Point For The Application Is Documented Below .

#### Process Text
- **POST** `/api/email/generate`
- **Description:** Sends the original email content and a desired tone to the backend for AI processing .
- **Request Body:**
  ```json
  {
  "emailContent": "Your original email text goes here...",
  "tone": "professional"
  }
  ```
- **Success Response (200 OK):**
  ```json
  {
  "reply": "The AI-generated reply will be in this field."
  }
  ```
## Future Roadmap

Some Features I'm Considering For Future Versions Include :

*   **Multi-language Support:** Enable reply generation for languages other than English .
*   **Custom Tones:** Allow users to define their own custom tones beyond the pre-defined options .
*   **Sentiment Analysis:** Analyze the sentiment of the original email to suggest an appropriate reply tone automatically .
*   **Calendar Integration:** Automatically detect meeting requests and suggest adding them to the user's calendar .
*   **Attachments:** The ability to handle and reference file attachments in replies .
*   **Desktop App:** Expand the application to a desktop version using frameworks like Electron .
---

