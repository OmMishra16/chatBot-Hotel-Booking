# Hotel Booking Chatbot

This is a RESTful API for a hotel booking chatbot using Express.js and OpenAI's API.

## Setup Instructions

1. Clone the repository
2. Run `npm install` to install dependencies
3. Create a `.env` file in the root directory and add your OpenAI API key:
4. Run `npm start` to start the server

## API Endpoints

### POST /api/chat

Send a message to the chatbot and receive a response.

Request body:
```json :- 
{
"userId": "unique_user_id",
"message": "I want to book a room"
}  

Response :- 
{
  "response": "Certainly! I'd be happy to help you book a room. Let me fetch the available room options for you."
}

Testing :- 
curl -X POST `http://localhost:3000/api/chat` \
  -H "Content-Type: application/json" \
  -d '{"userId": "user123", "message": "I want to book a room"}'

Continue the conversation by sending more messages with the same userId to maintain the conversation history.

To run the application, you'll need to:

1. Install the dependencies using `npm install`
2. Set up your OpenAI API key in the `.env` file
3. Start the server using `node app.js`

You can then interact with the chatbot by sending POST requests to `http://localhost:3000/api/chat` with the appropriate JSON body.
