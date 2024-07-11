---

# FoodieBot: A Conversational Food Ordering Chatbot

This project implements a Dialogflow-based chatbot for managing food orders. It allows users to add items to their order, remove items, complete orders for database storage, and track existing orders using a backend system.

## Features

- **Add to Order**: Allows users to add food items and quantities to their current order.
- **Remove from Order**: Enables users to remove specific items from their current order.
- **Complete Order**: Finalizes the current order, stores it in a database, and provides an order ID and total for payment.
- **Track Order**: Lets users check the status of an existing order by providing the order ID.

## Project Structure

- **`app.py`**: Main FastAPI application file handling webhook requests and routing to appropriate handlers.
- **`db_helper.py`**: Helper functions for database interactions, including inserting orders and retrieving order status.
- **`generic_helper.py`**: Utility functions such as extracting session IDs and formatting order details.
- **`requirements.txt`**: Lists all dependencies required to run the project.

## Setup Instructions

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/Anands001/DialogFlow---ChatBot.git
   cd YourRepository
   ```

2. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Application:**
   ```bash
   uvicorn app:app --reload
   ```

4. **Configure Dialogflow Webhook:**
   - Set up a Dialogflow agent.
   - Configure the webhook URL to point to your deployed FastAPI application.

## Usage

- **Adding to Order**:
  - Send a request to add food items using the appropriate intent.
- **Removing from Order**:
  - Specify items to remove from the current order.
- **Completing an Order**:
  - Finalize the order to store it in the database and receive payment details.
- **Tracking an Order**:
  - Provide the order ID to check its current status.

## Contributing

Contributions are welcome! Feel free to fork the repository and submit pull requests with improvements or additional features.

---
