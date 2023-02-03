# Automated tests Facebook login page By Lama
This repository contains automated tests for Facebook login page

## Setup

### Python
You will need a Python 3 interpreter installed on your machine to run the tests. For ease of use
a virtual environment is recommended. Install the dependencies from the `requirements.txt` file.


## Running the tests
Use the `robot` command to run the tests from the `TestCases` directory. It is important that you run the
command from the root of this project with the `--pythonpath .` option at the very least. This will
ensure that RobotFramework will find all the required keywords. A very useful option is the 
`--outputdir path/to/dir` option. It sets the directory where the html report and log will be generated. 
Normally this would be set to `Reports`.

```shell
robot --pythonpath . --outputdir Reports --variablefile vars.py path/to/robot/suite
```

Please see the Robot Framework [docs] for more details on command line options.

## Pipelines
The code has a pipeline to help run All Test Cases at 19:00

## Project structure
The project files have the following structure:
- `Var` - locators of elements of each view and page of each of the applications under test
- `Keywords` - Robot Framework custom keywords used to navigate through the applications
- `TestCases` - `.robot` files with defined test cases
- `.github` - Github information including pipeline definitions in `.yml` format.

[docs]: http://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#using-command-line-options
[this]: https://corese.atlassian.net/wiki/spaces/EXFP/pages/693960729/Test+Accounts