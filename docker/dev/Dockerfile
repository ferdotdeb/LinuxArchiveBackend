FROM python:3.14-slim

WORKDIR /app

RUN apt-get update && apt-get install -y --no-install-recommends git && rm -rf /var/lib/apt/lists/*

COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

# Para devcontainer lo mantiene vivo y luego ejecuta postStartCommand
CMD ["sleep", "infinity"]