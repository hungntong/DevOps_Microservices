FROM python:3.12.0a4-bullseye
LABEL maintainer="Udacity"

# Working Directory
WORKDIR /app

# Copy source code to working directory
COPY . hello.py /app/

# Install packages from requirements.txt
# hadolint ignore=DL3013
RUN pip install --upgrade pip &&\
    pip install --trusted-host pypi.python.org -r requirements.txt
    
RUN python --version

# Expose port 80
EXPOSE 80

# Run app.py at container launch
CMD ["python", "hello.py"]