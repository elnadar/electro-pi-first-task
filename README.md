## Project Description
- Python Script that would take any type of data as an input whether (.csv or .xlsx) that hold data with different type of errors that need to be corrected first then return an automated Exploratory Data Analysis Charts as an output.
- Sample Input : "data.xlsx"
- Desired Output: EDA for that data

## Run

```bash
$ python script.py -h
```

Output:
```text
usage: script.py [-h] [-l AUTOMATION_LEVEL] [-f FILE_PATH] [-a ARGUMENTS]
                 [-m MAXIMUM_NUM_OF_STRING_UNIQUE_VALUES]

optional arguments:
  -h, --help            show this help message and exit
  -l AUTOMATION_LEVEL, --automation-level AUTOMATION_LEVEL
                        Selecting the automation level: full: just choose the
                        file path and everything will be automated. high: also
                        lets you to assign value for arguments of the
                        `read_file` function. semi: also lets you choose
                        maximum num of unique values in any string column to
                        be selected in the EDA, its 100 by default. low: also
                        lets you choose columns to apply many choosen plots on
                        it. none: also lets you change types of columns to
                        apply specific plots on it.
  -f FILE_PATH, --file-path FILE_PATH
                        lets you to choose file path before the run
  -a ARGUMENTS, --arguments ARGUMENTS
                        lets you to assign value for arguments the `read_file`
                        function, eg: (-a sheet_name=sheet1). you can specify
                        many using comma - don't forget quotation -, eg: (-a
                        "sheet_name=sheet1, header=0"). * if you don't know
                        the parameter's names you can use --automation-level
                        argument and set it with "high" value.
  -m MAXIMUM_NUM_OF_STRING_UNIQUE_VALUES, --maximum-num-of-string-unique-values MAXIMUM_NUM_OF_STRING_UNIQUE_VALUES
                        lets you choose maximum num of unique values in any
                        string column to be selected in the EDA, its 100 by
                        default.
```

## Dependences
- numpy
- pandas
- inspect
- argparse
- matplotlib
- seaborn

you can install dependences using pip:
```bash
pip install numpy pandas inspect argparse  matplotlib seaborn
```

## Examples
You can see examples from `final_plots.ipynb` file.

