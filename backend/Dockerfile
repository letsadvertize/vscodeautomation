# Use Python 3.9 as base image
FROM python:3.9

# Set the working directory to /app
WORKDIR /app

# Copy the requirements.txt file from the backend folder into the container
COPY ./backend/requirements.txt .

# Install dependencies from requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of the backend application files
COPY ./backend/ .

# Expose port 5000
EXPOSE 5000

# Set the default command to run the Flask application
CMD ["python", "app.py"]
