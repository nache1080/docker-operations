# Use an official Python runtime as a parent image
FROM python:3.12-slim

# Set the working directory inside the container
WORKDIR /app

# Copy requirements file if you have one (optional)
# If you don't have requirements.txt, you can remove these two lines
COPY scripts/sample-deploy/requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy your Python script(s) into the image
COPY scripts/sample-deploy/app.py

# Run your script by default
# Replace "app.py" with your script name
CMD ["python", "app.py"]