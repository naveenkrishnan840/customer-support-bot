# Airbus Aircraft Customer Support Bot

<div align="center">
  <!-- Backend -->
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" />
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" />
  <img src="https://img.shields.io/badge/Faiss-4F5B93?style=for-the-badge&logo=faiss&logoColor=white" />
  <img src="https://img.shields.io/badge/Google-4285F4?style=for-the-badge&logo=google&logoColor=white" />
  <img src="https://img.shields.io/badge/DeepSeek-003A4D?style=for-the-badge&logo=deezer&logoColor=white" />
  <img src="https://img.shields.io/badge/LangChain-121212?style=for-the-badge&logo=chainlink&logoColor=white" />
  <img src="https://img.shields.io/badge/FlashrankRerank-4B9CD3?style=for-the-badge&logo=flash&logoColor=white" />
  <img src="https://img.shields.io/badge/LangGraph-FF6B6B?style=for-the-badge&logo=graph&logoColor=white" />
  
  <!-- Frontend -->
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />
  <img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" />
  <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black" />

  <h3>Your AI Co-pilot for Airbus Aircraft Customer Chat Bot 🚀</h3>

  <p align="center">
    <b>Autonomous Flight Booking Agent | Hostel Booking Agent | Car Rental Agent | Excursion Booking Agent | Customer Policy Information Retrieval </b>
  </p>
</div>

# Overview
The <b>Airbus Aircraft Customer Chat Bot </b> is an intelligent, multi-agent system that provides a seamless, efficient, and personalized experience for users booking flights, hotels, car rentals, and excursions. With its ability to access real-time data via MySQL, interact across multiple service categories, and use AI-powered NLP for context-driven conversations, this bot is a powerful tool for both customers and businesses. By leveraging advanced technologies, the bot helps streamline complex travel arrangements and delivers an exceptional customer experience.

# Motivation
Efficiency meets innovation. With the power of intelligent technology, you can navigate the complexities of travel with ease and confidence. The Airbus Aircraft Customer Chat Bot doesn’t just streamline your journey—it transforms it, offering you a personalized, seamless experience that lets you focus on what truly matters: enjoying the adventure ahead. Whether it’s booking flights, hotels, or planning exciting excursions, let technology be your trusted companion in making every step of your travel smarter and more enjoyable. Embrace the future of travel and make every moment count.

## Key Features

## Agent Capabilities
  ### 1. Primary Assistant
  The Primary Assistant is the central control hub that manages the conversation and directs queries to the appropriate agent based on user intent.
#### Capabilities:
  - Request Routing: Recognizes user queries and forwards them to the relevant assistant (Flight, Car Rental, Hotel, or Excursion Assistant).
  - Context Management: Keeps track of the ongoing conversation, ensuring that user queries are contextually linked and coherent even when switching between services.  
  - Multi-Agent Coordination: Orchestrates communication across different agents to deliver a unified response. It integrates information from multiple agents (e.g., flight     and hotel) to create a seamless user experience.
  - Intent Detection: Identifies the nature of the user’s request (e.g., booking a flight, reserving a hotel, renting a car) and triggers the appropriate agent.
    Personalized Recommendations: Provides suggestions based on user preferences, past interactions, or stored information across all agents.
##### Tools:
  - Route Query: Directs user questions to the appropriate assistant based on the service requested (Flight, Hotel, Car, Excursion).
  - Context Management: Tracks the conversation flow, manages the context, and keeps the user journey consistent.

### 2. Flights Assistant
  The Flights Assistant is responsible for assisting users with flight bookings, availability checks, and flight-related queries.

#### Capabilities:
  - Flight Search: Retrieves flight details from the MySQL database and shows available flights.
      Example:
      - QR0051: BSL to BKK, Scheduled for 2025-03-09 at 15:08 (departure) and 20:13 (arrival).
      - CA0065: GVA to DEN, Scheduled for 2025-03-11 at 15:33 (departure) and 20:13 (arrival).
      - BA0022: SEZ to SHA, Scheduled for 2025-03-01 at 17:33 (departure) and 23:23 (arrival).
      - Flight Booking: Allows users to book flights based on search results, entering user details (names, seats, preferences) into the system.
      - Flight Update: Users can request changes (e.g., date changes, seat selection) to booked flights.
      - Flight Cancellation: Enables users to cancel an existing flight reservation, either fully or partially.
##### Tools:
  - Search: Queries available flights from the database based on user input (e.g., departure date, source, and destination).
  - Book: Allows flight booking by processing user preferences and providing confirmation details.
  - Update: Facilitates modification of flight bookings, such as changing travel dates, or seat preferences.
  - Cancel: Manages cancellation of flight bookings and provides options to the user, including refund or rebooking.
### 3. Car Rental Assistant
  The Car Rental Assistant handles car rental searches, bookings, and changes related to rental vehicles.

#### Capabilities:
  1. Car Rental Search: Retrieves available car rental options based on user preferences and location.
     - Example:
         - Europcar (Economy) in Basel from 2024-04-14 to 2024-04-11.
         - Avis (Luxury) in Basel from 2024-04-10 to 2024-04-20.
         - Hertz (Midsize) in Zurich from 2024-04-10 to 2024-04-07.
         - Sixt (SUV) in Bern from 2024-04-20 to 2024-04-26.
  2. Car Rental Booking: Facilitates car rental booking based on available options, allowing users to select vehicle type, pickup/dropoff locations, and rental dates.
  3. Car Rental Update: Users can request changes to an existing car rental, such as altering the rental period or car type.
  4. Car Rental Cancellation: Provides the ability to cancel a car rental reservation, either entirely or for specific dates.
##### Tools:
  1. Search: Allows users to search for car rental availability based on location, vehicle type, and rental dates.
  2. Book: Facilitates car rental bookings, ensuring availability and confirming reservation details.
  3. Update: Manages changes to existing reservations, such as modifying pickup dates or vehicle categories.
  4. Cancel: Handles cancellations for car rental bookings and initiates refund processes when applicable.

## Agent Types

### 1. Primary Agent
A specialized automation agent for executing web-based tasks and workflows.
- Custom action planning for multi-step tasks
- Dynamic element interaction based on context
- Real-time task progress monitoring

### 2. Flight Booking Agent
An information gathering specialist with smart content processing.
- Intelligent source selection and validation
- Adaptive search refinement
- Single-pass comprehensive information gathering

### 3. hotel Booking Agent
An advanced research agent that produces academic-quality content through systematic topic exploration.
- Automatic topic decomposition and structured research
- Independent subtopic exploration
- Academic paper generation with proper citations
- Cross-referenced bibliography compilation

### 4. Car Rental Agent

### 5. Excursion Booking Agent


### Agent Architecture Diagrams

#### Deep multi Agent Work Flow
<img src="https://github.com/naveenkrishnan840/customer-support-bot/blob/main/graph.png"/>

*Multi Agent's workflow for comprehensive booking and content generation*

## Architecture

The system is built on a modern tech stack with three distinct agent types, each powered by:

1. **State Management**
   - LangGraph for maintaining agent state
   - Handles complex navigation flows and decision making
   - Structured workflow management

2. **Browser Automation**
   - Playwright for reliable web interaction
   - Custom element detection and interaction system
   - Automated navigation and content extraction

3. **Content Processing**
   - RAG (Retrieval Augmented Generation) pipeline
   - Vector store integration for efficient information storage
   - PDF and webpage content extraction
   - Automatic content structuring and organization

4. **AI Decision Making**
   - Multiple LLM integration (GPT-4, Claude)
   - Context-aware navigation
   - Self-review mechanisms
   - Structured output generation

## Setup Instructions

### Backend Setup

1. Clone the repository
   ```bash
   git clone https://github.com/hrithikkoduri18/WebRover.git
   cd customer_support_bot
   cd backend
   ```

2. Install Poetry (if not already installed)

   Mac/Linux:
   ```bash
   curl -sSL https://install.python-poetry.org | python3 -
   ```
   Windows:
   ```bash
   (Invoke-WebRequest -Uri https://install.python-poetry.org -UseBasicParsing).Content | python -
   ```

3. Set Python version for Poetry
   ```bash
   poetry env use python3.12
   ```

4. Activate the Poetry shell:
   For Unix/Linux/MacOS:
   ```bash
   poetry shell
   # or manually
   source $(poetry env info --path)/bin/activate
   ```
   For Windows:
   ```bash
   poetry shell
   # or manually
   & (poetry env info --path)\Scripts\activate
   ```

5. Install dependencies using Poetry:
   ```bash
   poetry install
   ```

6. Set up environment variables in `.env`:
   ```bash
   OPENAI_API_KEY="your_openai_api_key"
   LANGCHAIN_API_KEY="your_langchain_api_key"
   LANGCHAIN_TRACING_V2="true"
   LANGCHAIN_ENDPOINT="https://api.smith.langchain.com"
   LANGCHAIN_PROJECT="your_project_name"
   ```

7. Run the backend:

   Make sure you are in the backend folder

    ```bash
    uvicorn app.main:app --reload --port 8000 
    ```

   For Windows User:

    ```bash
    uvicorn app.main:app --port 8000
    ```

8. Access the API at `http://localhost:8000`

### Frontend Setup

1. Open a new terminal and make sure you are in the WebRover folder:
   ```bash
   cd frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Run the frontend:
   ```bash
   npm run dev
   ```

4. Access the frontend at `http://localhost:3000`

For mac users: 

Try running http://localhost:3000 on Safari browser. 
If you face any with connecting to browser, open terminal and run:

```bash
pkill -9 "Chrome"
```
and try again.

If you still face issues, try changing the websocket port from 9222 to 9223 in the `webrover_browser.py` file in the `backend/Browser` folder.


## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Made with ❤️ by [@naveenkrishnan840](https://github.com/naveenkrishnan840)
