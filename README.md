# Google Integration Portal

![Flask](https://img.shields.io/badge/Flask-1.1.2-blue.svg) ![React](https://img.shields.io/badge/React-17.0.2-blue.svg) ![Python](https://img.shields.io/badge/Python-3.12-blue.svg) ![License](https://img.shields.io/badge/License-MIT-green.svg)

A platform for users to view and manage their Google My Business reviews. The portal simulates the Google My Business API to fetch and display reviews, allowing users to respond directly from the interface.

---

## Key Features

- **Google Authentication:** Secure user access (mocked for now)
- **Review Management:** Fetch and display reviews, respond directly
- **Responsive Design:** Works across devices, offering a seamless experience

---

## 🛠️ Technical Stack

- **Backend:** Flask (Python)
- **Frontend:** (To be implemented) React or Node.js
- **API Integration:** Simulated Google My Business API
- **Authentication:** OAuth 2.0 (mocked)

---

## 🚀 Getting Started

### Prerequisites

To run the project locally, you’ll need:

- Python 3.12
- Flask
- JavaScript
- React (planned)
- Node.js (planned)

### Installation

Follow these steps to set up the project on your local machine:

```bash
# Clone the repository
git clone https://github.com/your-username/google-integration-portal.git

# Navigate to the project directory
cd google-integration-portal

# Install the required Python dependencies
pip install -r requirements.txt
```
## Running the Application
To start the Flask backend server, run:
```bash
python app.py
```
### Running the Frontend

To start the frontend (assuming a React setup), follow these steps:

1. **Navigate to the frontend directory (if separate):**

    ```bash
    cd frontend
    ```

2. **Install the required Node.js dependencies:**

    ```bash
    npm install
    ```

3. **Start the frontend development server:**

    ```bash
    npm start
    ```

The frontend will be available at [http://localhost:3000](http://localhost:3000) by default.

## API Endpoints

Here are the available API endpoints:

| Method | Endpoint                          | Description                                     |
|--------|-----------------------------------|-------------------------------------------------|
| GET    | `/api/reviews`                     | Fetches reviews (requires authentication)       |
| POST   | `/api/reviews/<review_id>/reply`   | Adds a reply to a review (requires authentication) |

## Frontend Integration 

To complete the frontend integration, the following tasks are planned:

- **User Authentication:** Implement authentication handling to secure user access.
- **Display Reviews:** Develop a user-friendly interface to show reviews effectively.
- **Reply Functionality:** Enable users to respond to reviews directly from the portal.

## Challenges and Future Enhancements

Future improvements and challenges include:

- **API Integration:** Replace the current dummy data with the actual Google My Business API.
- **Error Handling:** Enhance error handling and validation processes to ensure robustness.
- **Database Integration:** Integrate a database for managing user data, authentication tokens, and caching to improve performance and scalability.

## Dummy API Implementation

Currently, the project uses `DUMMY_DATA` to simulate API responses. Authentication is mocked and always returns `True`.

## Expected API Response Structure

For reference, the expected structure of the API response is:

```json
{
  "reviewId": "...",
  "reviewer": {
    "displayName": "...",
    "profilePhotoUrl": "..."
  },
  "comment": "...",
  "starRating": ...,
  "createTime": "...",
  "response": {
    "comment": "...",
    "updateTime": "..."
  }
}
```

### Breakdown:
- **`## Expected API Response Structure`**: Creates a level 2 heading for the section title.
- **Code Block with `json` Syntax Highlighting**: Displays the JSON structure in a formatted code block with syntax highlighting.


