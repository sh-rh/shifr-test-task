FROM python:3.12-slim

WORKDIR /api

COPY reqs.txt ./

RUN pip install --no-cache-dir --upgrade -r reqs.txt

COPY . ./api

CMD ["uvicorn", "api.main:app", "--host", "0.0.0.0", "--port", "8000"]