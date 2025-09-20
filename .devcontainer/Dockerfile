# Install Python 3.12
FROM mcr.microsoft.com/devcontainers/python:3.12

# Set working directory where Codespaces mounts the repository
WORKDIR /workspaces

# Prevent Python bytecode and enable unbuffered output
ENV PYTHONDONTWRITEBYTECODE=1
ENV PYTHONUNBUFFERED=1

# Copy requirements in cache
COPY requirements.txt /tmp/requirements.txt
RUN pip install --no-cache-dir -r /tmp/requirements.txt

# Expose Streamlit port
EXPOSE 8501
