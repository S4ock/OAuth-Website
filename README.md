# Flask OAuth Authentication App

This project demonstrates how to implement authentication in a Flask web application using OAuth 2.0 with Google, Twitter, and Facebook. The app allows users to log in via Google OAuth and includes a simple interface for interaction.

## Features

- **Google OAuth 2.0 Authentication**: Authenticate users via their Google accounts.
- **Twitter and Facebook OAuth (Coming soon)**: In progress for additional OAuth providers.
- **Custom Styled Login Page**: Simple, responsive UI with a custom background and hover effects.
- **Flask Framework**: Powered by Flask, a lightweight Python web framework.

## Getting Started

### Prerequisites

- Python 3.x
- Flask (`pip install Flask`)
- Authlib (`pip install Authlib`)

### Installation

1. Clone this repository to your local machine:
    ```bash
    git clone https://github.com/yourusername/your-repo.git
    ```

2. Navigate into the project directory:
    ```bash
    cd your-repo
    ```

3. Create a virtual environment and activate it:
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

4. Install the dependencies:
    ```bash
    pip install -r requirements.txt
    ```

5. Create a `.env` file in the root of the project and add the following:
    ```bash
    GOOGLE_CLIENT_ID=your-google-client-id
    GOOGLE_CLIENT_SECRET=your-google-client-secret
    ```

6. Run the Flask app:
    ```bash
    flask run
    ```

### Google OAuth Setup

1. Go to the [Google Developer Console](https://console.developers.google.com/).
2. Create a new project and enable **OAuth 2.0** for the project.
3. Add your **Client ID** and **Client Secret** to the `.env` file.
4. Set `http://localhost:5000/google/auth/` as the **Redirect URI** in the OAuth credentials.

### Usage

- Start the Flask app by running:
    ```bash
    python app.py
    ```
- Visit `http://localhost:5000` in your browser.
- Click on the **Login with Google** button to authenticate using your Google account.

### File Structure

```bash
.
├── app.py              # Main Flask application
├── templates/
│   └── index.html      # Frontend template
├── static/
│   └── bg.jpg          # Background image
├── requirements.txt    # Project dependencies
└── README.md           # Project documentation
