### Creation d'un dockerfile
Lancement d'un container de travail 
```
docker run -it ubuntu 
```{{execute T1}}

Tapez les commandes suivantes en sequence
mise a jour des repos d'ubuntu
```
apt-get update
```{{execute T1}}

Installation des packages python
```
apt-get -y install python3 python3-pip vim 
```{{execute T1}}

Installation de la libraire flask   
```
pip3 install flask
```{{execute T1}}

Copier le code dans cette commande
```
cat > /opt/app.py
```{{execute T1}}

```
python
# app.py
import os
from flask import Flask
app = Flask(__name__)

@app.route("/")
def main():
    return "Welcome!"

@app.route('/how are you')
def hello():
    return 'I am good, how about you?'

if __name__ == "__main__":
    app.run()
```







