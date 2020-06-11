# Fast API uploda file Demo

Fast api upload file demo app.

# Installation

```bash
virtualenv venv
source venv/bin/activate

(venv)$ pip install -r requirements.txt
(venv)$ uvicorn main:app --reload 
# INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)

```

# Usage

Curl can be used to send test this fast api. You can also use Rest clients like postman.

```bash

curl http://localhost:8000
# {"Hello":"World"}


curl -X POST -F "file=@C:\rmk\1.txt"  http://localhost:8000/uploadfile/
# {"filename":"1.txt"}

curl -X POST -F "file=@C:\rmk\1.txt" http://localhost:8000/files/
# {"file_size":24}


```
