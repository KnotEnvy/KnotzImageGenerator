# KnotzImageGenerator

KnotzImageGenerator is a sophisticated full-stack application that leverages OpenAI's DALL-E API to generate images from textual prompts.

## Project Overview

The application is composed of a backend server (`/server`) built with Node.js and a frontend interface (`/client`) built with React. The backend handles API calls, including requests to OpenAI's DALL-E API, and interacts with a MongoDB database to store posts. The frontend provides an interactive user interface for creating posts with image prompts and viewing the resulting images.

## Environment Variables

The application uses environment variables to handle sensitive data. The `.env` file should be located in the `/server` directory and include the following variables:

```
OPENAI_API_KEY=<your api key here>
MONGODB_URI=<your mongodb uri here>
```

Replace `<your api key here>` with your OpenAI API key and `<your mongodb uri here>` with your MongoDB connection string.

## Installation

1. Clone this repository to your local machine:

    ```sh
    git clone <repository url>
    ```

2. Navigate to the project directory and install the necessary dependencies:

    ```sh
    cd KnotzImageGenerator
    npm install
    cd client
    npm install
    cd ..
    cd server
    npm install
    ```

3. In the `/server` directory, create a `.env` file and add your OpenAI API key and MongoDB connection string.

## Usage

To start the application, run the server and client in separate terminals:

```sh
# In the /server directory
npm start

# In a new terminal, in the /client directory
npm start
```

The application will be available at `http://localhost:3000`.

## Troubleshooting

1. **Problem**: The application doesn't start or throws an error related to dependencies.
   **Solution**: Ensure that you have the latest version of Node.js and npm installed. If the problem persists, delete the `node_modules` folder and `package-lock.json` file in both the `/server` and `/client` directories, then run `npm install` again in each.

2. **Problem**: The application throws an error related to OpenAI API calls.
   **Solution**: Verify that your `.env` file is set up correctly with your OpenAI API key. Ensure that the key is correct and hasn't expired.

3. **Problem**: The application throws an error related to MongoDB.
   **Solution**: Check your MongoDB connection string in the `.env` file. Ensure that the string is correct and your MongoDB database is running.

## Contributing

We welcome contributions from the community. If you'd like to propose a significant change, please open an issue for discussion before submitting a pull request.
