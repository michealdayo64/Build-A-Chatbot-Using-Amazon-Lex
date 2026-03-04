# Build a Chatbot Using Amazon Lex
This is a demostartion of chatbot built using Amazon Lex. This mimics a banking chatbot where customer can ask for their account balance using prompt like their name and age. They can also make tranfer using the bot.

## Objective of the project
### 1️⃣ Build Your First Chatbot with Amazon Lex

### 2️⃣ Add Custom Slots to Your Lex Chatbot

### 3️⃣ Connect Your Lex Chatbot to Lambda

### 4️⃣ Save User Info with Your Lex Chatbot

### 5️⃣ Build Complex Conversations with Multiple Slots

## Build Your First Chatbot with Amazon Lex
- Here i was able to create an the bot basic that will interact with human.
<img width="1919" height="904" alt="Screenshot 2026-03-03 055542" src="https://github.com/user-attachments/assets/90c6db03-e709-4503-8841-32f21a0c654f" />

- Then i created an intent. An Intent is what the user is trying to achieve in their conversation with the chatbot. For example, checking a bank account balance; booking a     flight; ordering food.
<img width="1277" height="522" alt="Screenshot 2026-03-03 061106" src="https://github.com/user-attachments/assets/0fe558c6-da5d-4923-8af0-12bc03f4161c" />

- The responds on the Chatbot.
 <img width="530" height="725" alt="Screenshot 2026-03-03 061528" src="https://github.com/user-attachments/assets/61693123-c6e8-43bc-9d07-4a248d346cb8" />

- I configure a fallbackIntent just incase the bot does not understand the user message. It then respond with a user-friendly message.
<img width="441" height="669" alt="Screenshot 2026-03-03 063945" src="https://github.com/user-attachments/assets/b1bbb405-0fdc-4623-a471-5a820fa393ec" />


## Add Custom Slots to Your Lex Chatbot
- Here i created a slots that the user will use to get their account balance. E.g Account type and birthday slot.
<img width="994" height="461" alt="Screenshot 2026-03-04 074652" src="https://github.com/user-attachments/assets/f0ff5660-e652-43bb-9e41-d7b7b8ec34b1" />

- Then i set up intent to check account balance. Under the intent we add uttrances like "Check my account balace", "what is my account balance"
<img width="985" height="702" alt="Screenshot 2026-03-04 075901" src="https://github.com/user-attachments/assets/380405d2-3365-48d7-8389-62ab861b4a2b" />

##  Connect Your Lex Chatbot to Lambda
- Here we create a lambda function that run the backend code that respond to users requesting for their account balance.
  <img width="1452" height="610" alt="Screenshot 2026-03-04 090130" src="https://github.com/user-attachments/assets/ae57722b-172b-4ed8-8cc6-348370abf4ff" />

- Then i connected Amazon Lex to my newly created lambda using alias as a new version for my chatbot.
<img width="1105" height="616" alt="Screenshot 2026-03-04 092255" src="https://github.com/user-attachments/assets/b041db88-44cb-4825-98f9-186460727d18" />

- Following is Connect your CheckBalance intent with your Lambda function. This is done through fulfillment which select the lambda function
<img width="1577" height="880" alt="Screenshot 2026-03-04 093638" src="https://github.com/user-attachments/assets/468005c5-1e27-4247-a5ff-bdd5d9b762b0" />

