# Ecommerce Chatbot

The Ecommerce Chatbot is an enterprise-grade AI solution designed to revolutionize online shopping experiences. Built on Python and Flask framework, this sophisticated chatbot leverages advanced natural language processing (NLP) techniques to deliver intelligent, context-aware responses and personalized product recommendations. By seamlessly integrating with the e-commerce platform's product database, it provides real-time information on product availability, pricing, and shipping details, while maintaining a natural conversational flow that enhances customer engagement and satisfaction.

## Features

- **Intelligent Conversational Interface**
  - Real-time, context-aware chat interactions
  - Natural language understanding and processing
  - Multi-turn conversation management

- **Advanced Product Intelligence**
  - AI-powered product recommendation engine
  - Personalized suggestions based on user behavior
  - Dynamic pricing and availability updates

- **Seamless Database Integration**
  - Real-time product catalog synchronization
  - Efficient data retrieval and caching
  - Secure and scalable data management

- **Comprehensive Customer Support**
  - Instant response to product inquiries
  - Order tracking and status updates
  - Shipping and delivery information
  - Return and refund assistance

- **Enterprise-Grade Architecture**
  - High-performance request handling
  - Scalable cloud infrastructure
  - Secure data transmission
  - Continuous availability

## Installation

To set up the Ecommerce Chatbot locally, follow these steps:

1. Clone the repository to your local machine:
```
   git clone https://github.com/your-username/ecommerce-chatbot.git
```

2. Navigate to the project directory:
```
   cd ecommerce-chatbot
```

3. Install the required Python packages using pip:
```
pip install -r requirements.txt
```

4. Set up environment variables:
- Create a .env file in the project directory.
- Define the necessary environment variables such as database connection strings, API keys, etc.
  
5. Run the Flask application:
```
python app.py
```

## Set Up the Environment Variables

1. **Create a `.env` file** in the root directory of the project.

2. **Add the following keys** to the `.env` file and replace the placeholders with your actual credentials:

   ```ini
   GOOGLE_API_KEY=your_google_api_key_here
   ASTRA_DB_API_ENDPOINT=your_astra_db_endpoint
   ASTRA_DB_APPLICATION_TOKEN=your_astra_db_token
   ASTRA_DB_KEYSPACE=your_astra_db_keyspace
   ```

3. **Protect Sensitive Data**:
   - Add `.env` to your `.gitignore` file to prevent committing sensitive credentials:
     ```bash
     # .gitignore
     .env
     ```
   - ⚠️ Never share your `.env` file or upload it to version control (e.g., GitHub)

## AWS Deployment

Follow these steps to deploy the Ecommerce Chatbot on AWS EC2:

1. Push your code to GitHub:
   - Create a new repository on GitHub
   - Push your code using git commands

2. AWS EC2 Setup:
   - Log in to your AWS account
   - Launch an EC2 Instance
   - Configure your EC2 Instance

3. EC2 Instance Configuration:
   ```bash
   # Update package index
   sudo apt-get update
   sudo apt update -y

   # Install required tools
   sudo apt install git curl unzip tar make sudo vim wget -y

   # Clone your repository
   git clone <your-repository-url>

   # Create and configure .env file
   touch .env
   vi .env
   # Add your environment variables
   # Press 'i' to insert
   # Press 'Esc' to exit insert mode
   # Type ':wq' to save and exit

   # Verify .env contents
   cat .env

   # Install Python and pip
   sudo apt install python3-pip

   # Install project dependencies
   pip3 install -r requirements.txt --break-system-packages
   ```

4. Configure Security Group:
   - Go to EC2 Dashboard
   - Select your instance's Security Group
   - Add Inbound Rule:
     - Type: Custom TCP
     - Port Range: 5000
     - Source: 0.0.0.0/0 (Anywhere)
     - Description: Flask Application

5. Run the Application:
   ```bash
   python3 app.py
   ```

The application should now be accessible at `http://<your-ec2-public-ip>:5000`

## Setting Up Google Gemini API Key

To use the Google Gemini API in this project, you'll need to obtain an API key. Follow these steps:

1. Visit Google AI Studio:
   - Go to https://makersuite.google.com/app/apikey
   - Sign in with your Google account if you haven't already

2. Create a New API Key:
   - Click on "Create API Key" button
   - If this is your first time, you'll need to accept the terms of service
   - Your new API key will be displayed on the screen

3. Save Your API Key:
   - Copy the generated API key immediately
   - Store it securely as it won't be shown again
   - Add it to your `.env` file:
     ```
     GOOGLE_API_KEY=your_api_key_here
     ```

4. Important Notes:
   - Keep your API key secure and never commit it to version control
   - The API key has usage limits and quotas
   - Monitor your usage in the Google AI Studio dashboard
   - If you need to regenerate your key, you can do so from the API keys section

5. Usage Limits:
   - Free tier includes 60 requests per minute
   - Additional usage may require billing setup
   - Check current pricing and limits at https://ai.google.dev/pricing

For more information about the Gemini API, visit the official documentation at https://ai.google.dev/docs

## Setting Up Astra DB Credentials

To use DataStax Astra DB with this project, follow these steps to obtain and configure your database credentials:

1. Create a DataStax Account:
   - Visit https://astra.datastax.com/
   - Click "Sign Up" if you don't have an account
   - Complete the registration process

2. Create a New Database:
   - Log in to your Astra DB account
   - Click "Create Database"
   - Choose "Serverless" deployment type
   - Select your preferred cloud provider (AWS, GCP, or Azure)
   - Choose a region closest to your application
   - Enter a database name
   - Keep keyspace same 'default_keyspace' or
   - Create a keyspace with new name
   - Click "Create Database"

3. Get Your Database Credentials:
   - Once your database is created, click on it
   - Go to "Settings" tab
   - Click "Generate Token"

4. Configure Your Application:
   - Add these credentials to your `.env` file:
     ```
     ASTRA_DB_API_ENDPOINT='ASTRA_DB_API_ENDPOINT
     ASTRA_DB_APPLICATION_TOKEN='ASTRA_DB_APPLICATION_TOKEN'
     ASTRA_DB_KEYSPACE=default_keyspace(keep this same or choose your own in db)
     ```

5. Testing Your Connection:
   - After setting up credentials, test your connection
   - Monitor the Astra DB dashboard for any connection issues
   - Check your application logs for successful connection messages

For more information about Astra DB, visit the official documentation at https://docs.datastax.com/en/astra/

## System Architecture

### User Interface
![Chat Interface](https://raw.githubusercontent.com/your-username/ecommerce-chatbot/main/docs/images/chat-interface.png)
*Modern and intuitive chat interface for seamless user interaction*

![Dashboard View](https://raw.githubusercontent.com/your-username/ecommerce-chatbot/main/docs/images/dashboard.png)
*Admin dashboard for monitoring and managing chatbot operations*

### Database Architecture
![Database Schema](https://raw.githubusercontent.com/your-username/ecommerce-chatbot/main/docs/images/db-schema.png)
*Database schema showing relationships between different entities*

![Data Flow](https://raw.githubusercontent.com/your-username/ecommerce-chatbot/main/docs/images/data-flow.png)
*Data flow diagram illustrating the interaction between different system components*

Note: Replace the image URLs with actual paths to your project's images. The images should be stored in a `docs/images` directory within your repository.
