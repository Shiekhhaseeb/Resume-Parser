# Resume Parser

A FastAPI-based service for uploading and parsing resumes in PDF, DOC, DOCX, and TXT formats.

## Setup Instructions

> **Python Requirement:**  
> This project requires **Python 3.9**. Please ensure you have Python 3.9 installed before proceeding.

### 1. Clone the Repository

```sh
git clone git@github.com:Shiekhhaseeb/Resume-Parser.git
cd Resume-Parser
```

### 2. Create a Virtual Environment

```sh
python3.9 -m venv ../resume-parse-env
```

### 3. Activate the Virtual Environment

- **Linux/macOS:**
  ```sh
  source ../resume-parse-env/bin/activate
  ```
- **Windows:**
  ```sh
  ..\resume-parse-env\Scripts\activate
  ```

### 4. Install Dependencies

```sh
pip install --upgrade pip
pip install -r requirements.txt
```

### 5. Run the FastAPI Server

```sh
fastapi dev main.py
```

The API will be available at [http://127.0.0.1:8000](http://127.0.0.1:8000).

### 6. API Endpoints

- `POST /upload/` — Upload a resume file for parsing.
- `GET /` — Health check endpoint.

---

**Note:**  
- Only `.pdf`, `.doc`, `.docx`, and `.txt` files are allowed for upload.
- Uploaded files are stored in
