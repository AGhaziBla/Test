

# Utilise une image Python officielle comme base
FROM python:3.8-slim
RUN pip install scikit-learn
RUN pip install pandas

RUN mkdir -p mkdir ./app
# Définir le répertoire de travail dans le container
WORKDIR /app

# Copier les fichiers nécessaires dans le container
COPY Main.py /app/Main.py
COPY FS1.txt /app/FS1.txt
COPY PS2.txt /app/PS2.txt
COPY profile.txt /app/profile.txt

# Commande pour exécuter le programme Python
CMD ["python", "Main.py"]