# Certificate manager

## install

Execute the following line in Terminal to install prerequisites:

```
python3 -m pip install -r requirements.txt
```

Create a file `.getsecret.yaml` containing your postgres credentials:

```
POSTGRES_URL: <your postgres url>
```

## run the server

```
python3 server.py
```

## run the tests
Keep the server running, and execute the following line:
```
python3 tests.py
```

## Future TODOs:

Due to limited time, some features are not fully implemented.

* better error handling of the database query
* return a dictionary-like json body for every response and provide more informatic responses for POST/PATCH requests.
* return different status codes( 400, 404, etc.) for different types of errors and add correspondent tests for error handling
* add unit tests for db functionalities
* use a test framework for automated test