FROM python:3.9

# Set working directory
WORKDIR /app

# Copy the requirements file and install dependencies
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy the Python files and configuration file
COPY *.py .
COPY payment.ini .

# Expose the port
EXPOSE 8080

# Set environment variables
ENV AMQP_USER=roboshop \
    AMQP_PASS=roboshop123

# Run the application
CMD ["uwsgi", "--ini", "payment.ini"]
