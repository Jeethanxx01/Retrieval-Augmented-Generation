# 🛍️ Ecommerce Chatbot

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![Flask](https://img.shields.io/badge/Flask-2.0%2B-lightgrey)](https://flask.palletsprojects.com/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Active-success)]()

## 📂 Quick Navigation
- [View Project Images](Images/)
- [OpenAI Version of the Project](OpenAI_version/)

<div align="center">
  <img src="https://raw.githubusercontent.com/your-username/ecommerce-chatbot/main/docs/images/chat-interface.png" alt="Chat Interface" width="600"/>
</div>

## 🚀 Overview

The Ecommerce Chatbot is an enterprise-grade AI solution designed to revolutionize online shopping experiences. Built on Python and Flask framework, this sophisticated chatbot leverages advanced natural language processing (NLP) techniques to deliver intelligent, context-aware responses and personalized product recommendations. By seamlessly integrating with the e-commerce platform's product database, it provides real-time information on product availability, pricing, and shipping details, while maintaining a natural conversational flow that enhances customer engagement and satisfaction.

## ✨ Key Features

### 🤖 Intelligent Conversational Interface
- Real-time, context-aware chat interactions
- Natural language understanding and processing
- Multi-turn conversation management

### 🎯 Advanced Product Intelligence
- AI-powered product recommendation engine
- Personalized suggestions based on user behavior
- Dynamic pricing and availability updates

### 🔄 Seamless Database Integration
- Real-time product catalog synchronization
- Efficient data retrieval and caching
- Secure and scalable data management

### 💬 Comprehensive Customer Support
- Instant response to product inquiries
- Order tracking and status updates
- Shipping and delivery information
- Return and refund assistance

### 🏢 Enterprise-Grade Architecture
- High-performance request handling
- Scalable cloud infrastructure
- Secure data transmission
- Continuous availability

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

## 📊 System Architecture

### User Interface
<div align="center">
  <img src="https://raw.githubusercontent.com/your-username/ecommerce-chatbot/main/docs/images/chat-interface.png" alt="Chat Interface" width="400"/>
  <img src="https://raw.githubusercontent.com/your-username/ecommerce-chatbot/main/docs/images/dashboard.png" alt="Dashboard" width="400"/>
</div>

### Database Architecture
<div align="center">
  <img src="https://raw.githubusercontent.com/your-username/ecommerce-chatbot/main/docs/images/db-schema.png" alt="Database Schema" width="400"/>
  <img src="https://raw.githubusercontent.com/your-username/ecommerce-chatbot/main/docs/images/data-flow.png" alt="Data Flow" width="400"/>
</div>

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📧 Contact

For any queries or support, please reach out to [your-email@example.com](mailto:your-email@example.com)
