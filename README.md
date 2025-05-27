# 🛍️ Retrieval-Augmented Generation Ecommerce Chatbot

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![Flask](https://img.shields.io/badge/Flask-2.0%2B-lightgrey)](https://flask.palletsprojects.com/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Active-success)]()

## 📂 Quick Navigation
- [View Project Images](Images/)
- [OpenAI Version of the Project](OpenAI_version/)

## 🚀 Overview

AI-powered E-commerce Chatbot application leveraging Retrieval-Augmented Generation architecture that combines  
LLM capabilities to enable context-aware product recommendations and semantic search from real time vector Database.
Built with Python, Flask, Google's Gemini API, and DataStax Astra DB, and deployed on AWS EC2, this project marks a
revolution in e-commerce product recommendation domain.

## ✨ Key Features

### 🤖 Intelligent Conversational Interface
- Real-time  chat interactions
- Natural language understanding and processing

### 🎯 Advanced Product Intelligence
- AI-powered product recommendation engine
- Dynamic pricing and availability updates

### 🔄 Seamless Database Integration
- Real-time product catalog synchronization
- Efficient data retrieval  and scalable data management

### 🏢 Enterprise-Grade Architecture
- High-performance request handling
- Scalable cloud infrastructure

## 🛠️ Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/ecommerce-chatbot.git
   cd ecommerce-chatbot
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Configure environment variables**
   Create a `.env` file with the following structure:
   ```ini
   GOOGLE_API_KEY=your_google_api_key_here
   ASTRA_DB_API_ENDPOINT=your_astra_db_endpoint
   ASTRA_DB_APPLICATION_TOKEN=your_astra_db_token
   ASTRA_DB_KEYSPACE=your_astra_db_keyspace
   ```

4. **Run the application**
   ```bash
   python app.py
   ```

## ☁️ AWS Deployment

### Prerequisites
- AWS Account
- EC2 Instance
- Security Group Configuration

### Deployment Steps
1. **EC2 Instance Setup**
   ```bash
   sudo apt-get update
   sudo apt install git curl unzip tar make sudo vim wget -y
   git clone <your-repository-url>
   ```

2. **Environment Configuration**
   ```bash
   touch .env
   # Add your environment variables
   ```

3. **Install Dependencies**
   ```bash
   sudo apt install python3-pip
   pip3 install -r requirements.txt --break-system-packages
   ```

4. **Security Configuration**
   - Configure Security Group for port 5000
   - Allow inbound traffic from 0.0.0.0/0

5. **Launch Application**
   ```bash
   python3 app.py
   ```

## 🔑 API Configuration

### Google Gemini API
1. Visit [Google AI Studio](https://makersuite.google.com/app/apikey)
2. Create API Key
3. Add to `.env`:
   ```ini
   GOOGLE_API_KEY=your_api_key_here
   ```

### Astra DB Setup
1. Create account at [DataStax Astra](https://astra.datastax.com/)
2. Create new database
3. Generate token
4. Configure `.env`:
   ```ini
   ASTRA_DB_API_ENDPOINT=your_endpoint
   ASTRA_DB_APPLICATION_TOKEN=your_token
   ASTRA_DB_KEYSPACE=your_keyspace
   ```

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Authors

- **Jeethan Joel Crasta**-  [GitHub](https://github.com/Jeethanxx01)

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

Contributions are welcome! Please feel free to submit a Pull Request.

