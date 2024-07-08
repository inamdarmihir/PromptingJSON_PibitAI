# Resume PDF Parser

This Python script extracts text from a resume PDF file and uses the OpenAI API to parse the content into a structured JSON format. The structured data includes sections such as Personal Information, Summary, Education, Experience, Skills, Projects, and Certifications.

## Prerequisites

Before running the script, ensure you have the following installed:

- Python 3.x
- PyPDF2 library (`pip install PyPDF2`)
- OpenAI Python client (`pip install openai`)

You will also need:
- An OpenAI API key. You can obtain one from [OpenAI](https://www.openai.com/).
- A resume in PDF format (`resume.pdf`) that you want to parse.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/resume-pdf-parser.git
   cd resume-pdf-parser
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Set your OpenAI API key:

   Open `resume_pdf_parser.py` in a text editor and replace `'your-openai-api-key-here'` with your actual OpenAI API key.

## Usage

1. Place your resume PDF file (`resume.pdf`) in the same directory as `resume_pdf_parser.py`.

2. Run the script:

   ```bash
   python resume_pdf_parser.py
   ```

3. The script will:
   - Extract text from `resume.pdf`.
   - Use the extracted text as input to the OpenAI API to generate structured JSON data.
   - Print the parsed resume data in JSON format to the console.

## Output

The parsed resume data will be printed in the following JSON structure:

```json
{
    "personal_information": {
        "name": "",
        "email": "",
        "phone": "",
        "linkedin": "",
        "github": ""
    },
    "summary": "",
    "education": [
        {
            "degree": "",
            "institution": "",
            "graduation_year": ""
        }
    ],
    "experience": [
        {
            "job_title": "",
            "company": "",
            "duration": "",
            "responsibilities": [""]
        }
    ],
    "skills": [],
    "projects": [
        {
            "title": "",
            "description": "",
            "technologies": []
        }
    ],
    "certifications": [
        {
            "title": "",
            "issuing_organization": "",
            "date": ""
        }
    ]
}
```

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please create a GitHub issue or submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
