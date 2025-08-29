# buzzline-01-hanson

![Python 3.11](https://img.shields.io/badge/Python-3.11-blue?logo=python&logoColor=white)

This project introduces streaming data. 
The Python language includes generators - we'll use this feature to generate some streaming buzzline messages. 
As the code runs, it will continuously update the log file. 
We'll use a consumer to monitor the log file and alert us when a special message is detected. 

## Task 1. Set Up Your Machine & Sign up for GitHub

We practice professional Python. In each course that uses Python, we use a standard set of popular professional tools. 
This course uses advanced tools such as Apache Kafka that requires **Python 3.11**. 

## Task 2. Set Up Your Python Environment

Windows Powershell:

```shell
py -3.11 -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
```

## Task 3. Generate Streaming Data (Terminal 1)

Now we'll generate some streaming data. 

In VS Code, open a terminal.
Use the commands below to activate .venv, and run the generator as a module. 
To learn more about why we run our Python file as a module, see [PYTHON-PKG-IMPORTS](docs/PYTHON-PKG-IMPORTS.md) 

Windows PowerShell:

```shell
.venv\Scripts\activate
py -m producers.basic_producer_case
```

## Task 4. Monitor an Active Log File (Terminal 2)

A common streaming task is monitoring a log file as it is being written. 
This project has a consumer that reads and processes our own log file as log messages arrive. 

In VS Code, open a NEW terminal in your root project folder. 
Use the commands below to activate .venv, and run the file as a module. 

Windows:
```shell
.venv\Scripts\activate
py -m consumers.basic_consumer_case
``` 

## Task 5: Create and Monitor a Custom Active Log File

Copy over the contents of basic_producer_case.py to a new file (basic_producer_hanson.py) and modify the contents of the custom messages. Do the same with the basic_consumer_case.py file, except this time don't make any additions or modifications. 

## License
This project is licensed under the MIT License as an example project. 
You are encouraged to fork, copy, explore, and modify the code as you like. 
See the [LICENSE](LICENSE.txt) file for more.
