# Devops-p02
https://github.com/fporbor/Devops-p02.git

sudo systemctl restart docker.service

sudo systemctl restart networking.service

python3 -m venv venv

source venv/bin/activate

pip install -r requirements.txt

python src/app.py 

curl http://localhost:5000

gunicorn --chdir src app:app --bind 0.0.0.0:5000

docker build -t portgasdfran/galeria:latest .

docker push portgasdfran/galeria:latest

docker run -d -p 80:5000  --name testgaleria portgasdfran/galeria

curl http://localhost/status

docker stop testgaleria && docker rm testgaleria

docker compose  up -d       

curl http://localhost

docker compose down

docker push portgasdfran/galeria:latest 