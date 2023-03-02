setup:
	python3 -m venv ~/.udacity-devops

install:
	pip install --upgrade pip && pip install -r requirements.txt

lint:
	hadolint Dockerfile
	pylint --disable=R,C,W1203 **.py

all: 
	install lint test