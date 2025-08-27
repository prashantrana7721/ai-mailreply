# AI-Summarizer Assistant

A Powerful Browser-Based Tool Designed To Streamline Your Knowledge Processing . Leveraging The Power Of Google's Gemini AI , This Application Can Summarize Long Articles , Extract Key Points And Perform Other Content Operations Directly In Your Browser .

---

## Live Demo & Screenshots

Here Is A Look At The AI-Summarizer In Action , Summarizing A News Article About Cheteshwar Pujara's Retirement And A View Of The Backend API Being Tested With Postman .

#### Frontend in Action

*The Application's Sidebar Seamlessly Integrates With Any Webpage Allowing For On-The-Fly Text Summarization .*
<img src="images/news.png" alt="News">
<img src="images/extension.png" alt="Extension Working">


<br/>

#### Backend API Testing
*The Robust Spring Boot Backend Handles The Core Logic , Communicating With The Gemini API To Process Content . The Endpoint Is Tested And Validated Using Postman .*
<img src="images/request.png" alt="Api Testing Request">
<img src="images/response.png" alt="Api Testing Response">


---

## Core Features

*   **AI-Powered Summarization:** Instantly Condense Long Articles And Texts Into Concise Summaries .
*   **Seamless Integration:** Works As A Simple And Intuitive Sidebar In Your Browser .
*   **Extensible Operations:** The Backend Is Designed To Easily Support More Operations In The Future ( e.g - Keyword Extraction , Tone Analysis ) .
*   **Robust Backend:** Built With Java And Spring Boot For A Scalable And Reliable Service .
*   **RESTful API:** A clear And Well-Defined API For Processing Requests .

---

## Tech Stack

This Project Is Built With A Modern And Robust Set Of Technologies :

*   **Back-End:** Java 17 , Spring Boot , Spring Web , Maven
*   **AI Service:** Google Gemini Pro API
*   **Front-End:** HTML , CSS , JavaScript
*   **Testing & Tools:** Postman , Git , IntelliJ IDEA

---

## Getting Started

To Get A Local Copy Up And Running , Follow These Simple Steps :

### Prerequisites

*   **Java Development Kit (JDK) 17** or newer.
*   **Apache Maven**
*   **Git** for version control.
*   A **Google Gemini API Key**. You can get one from [Google AI Studio](https://aistudio.google.com/app/apikey).

### Installation & Configuration

1.  **Clone The Repository :**
    ```sh
    git clone https://github.com/your_username/ai-summarizer.git
    cd ai-summarizer
    cd aisummarizer-assistant-backend
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
    Use Maven To Run The Application . The Server Will Start On `localhost:8080` .
    ```sh
    chmod +x mvnw
    ./mvnw spring-boot:run
    ```

2.  **Load The Front-End :**
    *This Section Depends On Your Front-End Implementation . For A Browser Extension :*
    *   Open Your Browser ( e.g - Chrome ) .
    *   Navigate To `chrome://extensions` .
    *   Enable "Developer Mode".
    *   Click "Load Unpacked" And Select The Front-End Directory Of This Project .

---

## API Endpoint

The Primary API End-Point For The Application Is Documented Below .

#### Process Text
- **POST** `/api/research/process`
- **Description:** Sends Content And A Requested Operation To The Backend For AI Processing .
- **Request Body:**
  ```json
  {
      "content": "Your Long Text To Be Processed Goes Here...",
      "operation": "summarize"
  }
  ```
- **Success Response (200 OK):**
  ```json
  {
      "result": "The Summarized Version Of Your Text Appears Here ."
  }
  ```
## Future Roadmap

This Project Is A Living Work And I'm Excited About Its Future Potential . Some Features I'm Considering For Future Versions Include :

*   **Keyword Extraction:** Automatically Identify And List The Most Important Terms In A Text .
*   **Multi-Language Support:** Enable Summarization For Languages Other Than English .
*   **Custom Prompts:** Allow Users To Define Their Own Operations Beyond "summarize" ( e.g - " Explain This To Me Like I'm Five " ) . 
---

