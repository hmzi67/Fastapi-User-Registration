FROM python:3.12
LABEL maintinance="hamzawaheed057@gmail.com"
RUN pip install poetry
WORKDIR /code/
COPY . /code/
RUN poetry install
CMD [ "poetry", "run", "uvicorn", "sign_up.main:app", "--host", "0.0.0.0", "--reload" ]