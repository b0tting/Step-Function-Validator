# Step Function Validator for e.g. (AWS)

An issue we have is that we are quite human and we often make mistakes in the YAML "code". 
These could be syntactical errors (for example, an incorrect indent), but also semantical (for example, forgetting to add a required parameter to a step). 
We only find out about these errors in the last step of the CI/CD, when the step function fails to deploy to AWS. This makes troubleshooting very.. slow...

So we came up with this little tool. 

## Authors

- [@b0tting](https://github.com/b0tting)
- [@NileshDebix](https://github.com/NileshDebix)


## Installation

1. create virtual environment in python and activate this one in Terminal or CMD

```python
  python3 -m venv env
  
  Windows: 
    
    env\Script\activate.bat

  Mac/Linux:

    source env/bin/activate
```

2. pip install the tool via pypi

```python
    ####################### [ NOTE !!! ] ############################################################
    #    you NEED to see in your command line the env before your prompt
    #    so you know that you are in your virtual environment:
    #
    #    example: (env) niels@Mac%
    ################################################################################################

    if above is clear then:

    pip install stepfunction-validator or pip3 install stepfunction-validator # to install the required libraries and the tool

```


## Usage/Examples

```python
    YAML validator for the CLI

    Example: python app.py -c <test.yaml> [-s <stepfunctions_schema.json>] [--no-lint]
    This will validate a YAML file against the schema you provided in the CLI
```

