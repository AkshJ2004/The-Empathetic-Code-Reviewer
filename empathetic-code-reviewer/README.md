# Empathetic Code Reviewer

This tool generates a supportive, mentor-like code review report using the Groq API and Llama3 model.

## Prerequisites
- Python 3.10 or newer
- Internet connection (for API calls)
- `requests` Python package

## Setup
1. **Clone or download this repository.**
2. **Install dependencies:**
   Open a terminal in the project folder and run:
   ```powershell
   python -m pip install requests
   ```
3. **Prepare your input:**
   - Edit `input_data.json` and paste your code snippet and review comments in the following format:
     ```json
     {
       "code_snippet": "<your code here>",
       "review_comments": [
         "Comment 1",
         "Comment 2"
       ]
     }
     ```
   - Leave the file empty if you want others to fill it in later.

## How to Run
1. Open a terminal in the project directory.
2. Run the script:
   ```powershell
   python main.py input_data.json
   ```
   (If you are using a specific Python path, use that instead of `python`.)
3. The output will be saved to `report.md` in the same folder.

## Notes
- The script uses the Groq API and requires a valid API key (already set in the code).
- Make sure your input JSON is valid and contains the required fields.

## Example
See the sample format above for how to structure your input.

---
Feel free to modify `input_data.json` and rerun the script for different code reviews.
