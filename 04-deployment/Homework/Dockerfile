FROM python:3.13


# Set work directory
WORKDIR /app

# Copy your script into the container
COPY script.py .
COPY model.bin .

# If you have any dependencies in a requirements.txt file, copy that in as well
COPY requirements.txt .

# Install any required packages
RUN pip install --no-cache-dir -r requirements.txt

# Run script
CMD [ "python", "script.py", "2023", "5" ]