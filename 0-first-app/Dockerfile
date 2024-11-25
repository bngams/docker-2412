FROM public.ecr.aws/docker/library/python:3.14.0a2-slim-bullseye

# Récupérer code ou exec.
COPY requirements.txt my-requirements.txt

# Config. l'env, installer deps... 
RUN pip install -r my-requirements.txt

COPY src/index.py .

# Exec. au lancement contaier 
CMD ["python", "index.py"] 