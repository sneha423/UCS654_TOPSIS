UCS654 TOPSIS – 3 Part Assignment
This repository implements the TOPSIS method in three parts: CLI script, Python package, and a small web app

Part 1 – CLI Script
Folder: part1_cli
Run:

```
python topsis.py <input_file> <weights> <impacts> <output_file>
```

# example

```
python topsis.py data.csv 1,1,1,2 +,+,-,+ result.csv
```

Part 2 – Python Package
Folder: part2_package
Install:

```
pip install Topsis-sneha-102303033
```

Use:

```
from topsis_sneha_102303033 import topsis
topsis("input.csv", "1,1,1,2", "+,-,+,+", "output.csv")
```
link for python package: https://pypi.org/project/Topsis-sneha-102303033/

Part 3 – Web App
Folder: part3_web
Features:
Upload CSV
Enter weights and impacts
Enter email
Server runs TOPSIS and emails the result file.​
Configure email (example using environment variables):

# Windows PowerShell

```
$env:MAIL_USERNAME="your_project_email@gmail.com"
$env:MAIL_PASSWORD="your_app_password"
```

Run:

```
cd part3_web
python app.py
```

Open http://127.0.0.1:5000 and use the form.
