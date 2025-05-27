🚧 Pothole Detection and Reporting System

An intelligent web-based system for real-time pothole detection, severity analysis, and reporting using AI. Citizens can report potholes with location, images, and details. The system provides estimated pothole size, severity, traffic flow impact, and assigns bounty rewards — all backed by a Spring Boot REST API and a React frontend.📸 Features
🌍 Location tagging using Mapbox
The Project made us stand among the top 10 of 63 teams shortlisted from 400+ teams in Social Hackathon- An National Hackathon
📷 Image upload with real-time preview

🧠 AI-based analysis (Severity, Size, Traffic Flow)

💰 Dynamic bounty generation

📈 Success dashboard with all details

⚙️ Spring Boot API backend

☁️ Global accessibility (ESP32-compatible architecture ready for IoT)

🛠️ Tech Stack
Frontend	Backend	Other
React + TailwindCSS	Spring Boot (Java)	Mapbox API
ShadCN/UI	RESTful APIs	Multipart File Upload
Framer Motion	OpenAI (optional)	Google Maps (alternative)

🚀 Getting Started
📦 Clone the repository
bash
git clone https://github.com/yourusername/pothole-reporting-system.git
cd pothole-reporting-system

🧩 Frontend Setup
bash
cd frontend
npm install
npm start

⚙️ Backend Setup
bash
cd backend
./mvnw spring-boot:run

Configure your application.properties:
properties

spring.servlet.multipart.max-file-size=10MB
spring.servlet.multipart.max-request-size=10MB
spring.cors.allowed-origins=http://localhost:3000
📡 API Endpoints
Method	Endpoint	Description
POST	/api/report	Uploads pothole report and returns analysis
GET	/api/reports	Get all pothole reports (admin)

📊 AI Output Fields
Severity → Low, Moderate, Severe

Estimated Size → e.g., 58cm x 34cm

Traffic Flow → Light, Moderate, Heavy

Bounty → ₹ based on severity and traffic

📁 Project Structure
bash
/backend
 └── src/main/java/com/pothole/...
     ├── controllers
     ├── services
     ├── models
     └── repositories

/frontend
 ├── src/
 │   ├── components/
 │   ├── App.tsx
 │   └── index.tsx
 └── public/
🧪 Sample JSON Response
json
{
  "severity": "Moderate",
  "estimatedSize": "58 cm x 34 cm",
  "trafficFlow": "Heavy",
  "bounty": 1400
}
✨ Contributors
👨‍💻 Pulkit – Frontend, AI Integration

🤝 Tanmay – Backend, REST APIs

📜 License
This project is licensed under the MIT License – see the LICENSE file for details.
