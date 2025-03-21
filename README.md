# CertificadoAuto: Certificate Generation Automation

A Python automation tool that generates course certificates by pulling participant data from Excel spreadsheets.

## Overview
This project automates the process of generating certificates for course participants. The system reads participant data from an Excel spreadsheet, including names, course details, and dates, then places this information onto a certificate template image at precise coordinates with appropriate fonts.

## Features
- Reads participant data from Excel files
- Applies data to certificate template with proper positioning
- Uses custom fonts for professional appearance
- Automatically generates individual certificate files
- Handles multiple certificate types with consistent formatting

## Requirements
- Python 3.6+
- Required libraries:
  - openpyxl
  - Pillow (PIL)
  
## Installation
1. Clone this repository:
```
git clone https://github.com/yourusername/CertificadoAuto.git
cd CertificadoAuto
```

2. Install required packages:
```
pip install openpyxl pillow
```

3. Prepare your assets:
   - Place your Excel spreadsheet as `planilha_alunos.xlsx` in the project directory
   - Place your certificate template as `certificado_padrao.jpg` in the project directory
   - Ensure font files (`tahoma.ttf` and `tahomabd.ttf`) are in the project directory

## Excel File Structure
Your Excel file should have the following columns:
- Column A: Course Name
- Column B: Participant Name
- Column C: Participation Type
- Column D: Start Date
- Column E: End Date
- Column F: Hours (Workload)
- Column G: Issue Date

## Usage
1. Run the script:
```
python app.py
```

2. The script will:
   - Process each participant from the Excel file
   - Generate individual certificate images
   - Save files named with the pattern `{index}_{participant_name}_certificado.png`

## Customization
You can adjust the following parameters to match your certificate template:
- Font types and sizes
- Text coordinates on the certificate
- Output file naming pattern



## Important Notes
- The sample data in this repository is fictional and for demonstration purposes only
- Adjust text positioning coordinates if using a different certificate template

## License
6HTR66. This is a demonstration version project. All rights reserved.

## Contributing
Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/yourusername/CertificadoAuto/issues).
