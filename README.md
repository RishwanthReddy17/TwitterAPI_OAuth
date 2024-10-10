# TwitterAPI_OAuth
This project demonstrates how to post and delete tweets on Twitter using the Twitter API, OAuth 1.0a, and Golang.
- **Post a tweet** with a unique timestamp.
- **Delete a tweet** by specifying the tweet ID.
- Uses **OAuth 1.0a** for secure authentication with the Twitter API.
- Reads API credentials from a `.env` file for enhanced security.

## Setup Instructions

### Step 1: Create a Twitter Developer Account
1. Go to the [Twitter Developer Portal](https://developer.twitter.com/).
2. Log in with your Twitter account.
3. Click on **"Create an App"**.
4. Fill out the necessary details like app name, use case, etc.
5. After creating the app, navigate to the **"Keys and Tokens"** tab.

### Step 2: Generate API Keys
1. In the **"Keys and Tokens"** section, you’ll see:
   - **API Key (Consumer Key)**
   - **API Secret Key (Consumer Secret)**
2. Scroll down to **Access Token & Secret** and click on **"Generate"** to get:
   - **Access Token**
   - **Access Token Secret**
3. Copy these values and store them in a `.env` file (explained below).

### Step 3: Set Up `.env` File
1. Create a `.env` file in the root of your project directory.
2. Add the following content to the `.env` file:

    ```
    CONSUMER_KEY=your_consumer_key
    CONSUMER_SECRET=your_consumer_secret
    ACCESS_TOKEN=your_access_token
    ACCESS_SECRET=your_access_secret
    ```

### Step 4: Install Dependencies
Run the following commands to install necessary Go dependencies:
```
go get github.com/dghubble/oauth1
go get github.com/joho/godotenv

```

### Step 5: Running the Program
```
go run main.go

```
