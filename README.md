# Jenkins Multibranch Pipeline Project

This project demonstrates a Jenkins Multibranch Pipeline setup for a Python application.

## Project Structure

- `app.py`: Main application script.
- `test_app.py`: Contains unit tests for `app.py`.
- `Jenkinsfile`: Configuration for Jenkins pipeline.
- `README.md`: Project documentation.

## Prerequisites

- Python 3.x
- Jenkins with Multibranch Pipeline Plugin

## Setup Instructions

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/KevDen01/Jenkins-Python-Multibranch-Pipeline.git
   cd Jenkins-Python-Multibranch-Pipeline
   ```

2. **Create and Activate a Virtual Environment:**

   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows, use venv\Scripts\activate
   ```

3. **Install Dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

   *Note: Ensure `requirements.txt` lists all necessary packages.*

## Running the Application

```bash
python app.py
```

## Running Tests

```bash
python -m unittest test_app.py
```

## Jenkins Pipeline Setup

1. **Create a Multibranch Pipeline Job:**

   - In Jenkins, create a new Multibranch Pipeline job.
   - Set the repository URL to this project's GitHub repository.

2. **Configure Branch Sources:**

   - Add the repository as a branch source.
   - Set up credentials if necessary.

3. **Define Build Triggers:**

   - Configure triggers as per your requirements (e.g., periodic scans, webhook triggers).

4. **Pipeline Execution:**

   - Jenkins will automatically detect branches with a `Jenkinsfile` and execute the defined pipeline.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request.
