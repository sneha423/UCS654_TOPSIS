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

Upload CSV (first column: option names, remaining columns: numeric criteria)

Enter weights and impacts

Optional email field

Server runs TOPSIS and:

Shows the ranked result table on the page

Sends the result CSV as an email attachment (if email is provided)

Allows the user to download result.csv directly from the page

Deployed URL:
<https://topsis-web-vercel.vercel.app/>
