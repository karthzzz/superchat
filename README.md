# SuperChat

SuperChat is a simple chat application that allows users to send messages to each other in real-time. The application is built using React and Firebase.

The application is hosted on Firebase and can be accessed [here](https://superchat-7ae2d.web.app/).

## Features

- Real-time messaging
- Google authentication
- Profanity filtering
- Responsive design

## ToDo

- Implement LLMs to text each other instead of humans just sending messages.

## Getting Started

### Prerequisites

- Node.js
- npm

### Installation

1. Clone the repository:
	```bash
	git clone https://github.com/yourusername/superchat.git
	cd superchat
	```

2. Install dependencies:
	```bash
	npm install
	```

### Available Scripts

In the project directory, you can run:

- `npm start`: Runs the app in the development mode. Open [http://localhost:3000](http://localhost:3000) to view it in your browser.
- `npm test`: Launches the test runner in the interactive watch mode.
- `npm run build`: Builds the app for production to the `build` folder.

### Firebase Functions

The project includes a Firebase function to detect and filter profanity in messages. The function is defined in `functions/index.js`.

### Deploying Firebase Functions

1. Install Firebase CLI:
	```bash
	npm install -g firebase-tools
	```

2. Login to Firebase:
	```bash
	firebase login
	```

3. Deploy functions:
	```bash
	firebase deploy --only functions
	```

### GitHub Actions

The project uses GitHub Actions for continuous deployment. The workflows are defined in the `.github/workflows` directory.

- `firebase-hosting-pull-request.yml`: Deploys to Firebase Hosting on pull requests.
- `firebase-hosting-merge.yml`: Deploys to Firebase Hosting on merge to the master branch.

### Project Structure

#### Key Files

- `src/App.js`: Main application component.
- `src/App.css`: Styling for the application.
- `src/index.js`: Entry point for the React application.
- `functions/index.js`: Firebase functions for backend logic.

### Learn More

To learn React, check out the [React documentation](https://reactjs.org/).

To learn Firebase, check out the [Firebase documentation](https://firebase.google.com/docs).

### License

This project is licensed under the MIT License.