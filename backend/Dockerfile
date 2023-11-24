from python:3-alpine3.15
workdir /app
copy . /app
run pip install --upgrade pip
# run python3 -m pip install -r requirements.txt
run apt install -y ffmpeg
run python -m pip install --pre --upgrade vosk==0.3.45
run uvicorn main:app --host 0.0.0.0 --port 8080