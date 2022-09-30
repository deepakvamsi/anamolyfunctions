
# IoT Functions

A companion package to IBM Watson IoT Platform Analytics containing sample functions and base classes from which to derive custom functions.

## Getting Started

These instructions will get you up and running in your local environment or in Watson Studio for development and testing purposes. 

### Prerequisites

 + python 3.X (https://www.anaconda.com/distribution/)
 + future (pip install future)
 + pandas (pip install pandas)
 + sqlalchemy (pip install sqlalchemy)
 + lxml (pip install lxml)

### Build and Shipment

**Caveat**
- Shipping to pypi or test-pypi requires a token
- Version numbers can never be reused.

1. Build a distribution first
    ```
    python3 setup.py sdist bdist_wheel
    ```
2. Upload to test-pypi
    ```
    twine upload --verbose --repository testpypi dist/*
    ```
3. When everything appears to be okay upload to pypi
    ```
    twine upload --verbose --repository pypi dist/*
    ```

### Installing

1. Create a virtual environment
    ```
    python3 -m venv env
    ```
2. Activate virtual environment
    ```
    source env/bin/activate
    ```
3. Install in your local environment from GitHub
   ```
   pip install git+https://github.com/deepakvamsi/anomaly-uml
   ```

To install in IBM Watson Studio from another Jupyter notebook:

```~~~bash
!pip install git+https://github.com/deepakvamsi/anomaly-uml
```

Test for successful install:

```~~~python3
import iotfunctions as fn
print(fn.__version__) 
```



### Further information 
+ [Sample Notebook](https://www.ibm.com/support/knowledgecenter/SSQP8H/iot/analytics/as_notebook_references.html) 


