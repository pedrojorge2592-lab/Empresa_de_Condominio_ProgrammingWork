🏢 Condominium Maintenance & Repair Management System

This project provides a Python-based system for managing condominium repairs. It combines automation with an AI-powered chatbot (Ollama) to streamline the process of reporting issues, assigning engineers, and tracking repair status.

📌 Project Overview

Goal: Simplify maintenance management in condominiums by automating issue reporting and engineer assignment.

Key Features:

Residents report problems in apartments (plumbing, electricity, etc.).

Ollama chatbot understands natural language reports and classifies the issue.

Python script automatically schedules an engineer based on availability & specialization.

Notifications sent to both the resident and the assigned engineer.

Task tracking until completion.

🛠️ Architecture

User Input: Resident describes the problem (text/chat).

Chatbot (Ollama):

NLP to understand the issue.

Categorizes problem (e.g., plumbing, electrical, structural).

Task Scheduler (Python):

Searches engineer database.

Matches specialization with problem type.

Assigns the next available engineer.

Database: Stores residents, issues, engineers, and schedules.

Notifications: Task confirmation sent to stakeholders.

🗂 Repository Contents

maintenance_scheduler.py → Python script for assigning engineers.

chatbot_integration.py → Ollama chatbot interface.

engineers.csv → Engineer database (names, roles, availability).

tasks.db → SQLite database for tracking repair tasks.

README.md → Project documentation.

🛠️ Technologies Used

Python (automation & scheduling)

SQLite / PostgreSQL (task management database)

Ollama (chatbot NLP for issue classification)

Flask / FastAPI (optional API for deployment)

Pandas / Numpy (data handling)

🚀 How to Run

Clone the repository:

git clone https://github.com/yourusername/CondoRepairSystem.git
cd CondoRepairSystem


Install dependencies:

pip install -r requirements.txt


Start the chatbot & scheduler:

python chatbot_integration.py
python maintenance_scheduler.py


Report a problem (example):

"My bathroom sink is leaking."  
→ Chatbot: Issue classified as **Plumbing**  
→ Engineer John assigned, scheduled for tomorrow at 10:00 AM.  

📈 Features in Action

🤖 AI-powered issue classification – Residents can write problems naturally.

👷 Engineer matching – Right specialist is assigned automatically.

📅 Scheduling system – Avoids conflicts and ensures efficient resource use.

📊 Tracking & reporting – Managers can see open, ongoing, and completed repairs.

📌 Future Improvements

Mobile app for residents to report issues with photos.

Integration with billing system for repair costs.

Predictive maintenance using IoT sensors in apartments.

Expand chatbot knowledge base to handle FAQs.

👨‍💻 Author

Pedro Silva
