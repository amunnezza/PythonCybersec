
#### per creare un virtual environment usa il comando
_python -m venv .venv_ 
#### dove .venv lo usi cosi viene escluso da git ed è dir di installazione
#### per attivare usi poi in linux 
_source .venv/bin/activate_

#### installi requirements con
_pip install -r requirements.txt_


#### Per iniziare puoi avere dei problemi con l'installazione dei requirements.
#### Principalmente il problema lo pone la libreria libratom
#### Non trova il compilatore e la soluzione puo essere installare il compilatore che si installa con

_sudo apt update && sudo apt upgrade_

_sudo apt-get install g++_ 

_sudo apt-get install python3-dev_
#### libreria c++ che necessaria
_pip install setuptools wheel_

_pip install libratom_

#### che risolve

#### PASSANDO ALLA PARTE git
#### Chiaramente installi git se non presente
_sudo apt install git_

#### settaggi iniziali 
_git config --global user.email "amunnezza@gmail.com"_

_git config --global user.name "amunnezza"_

#
#### aggiungi i file e aggiungi come remote il repository github.com 
_git add ._

_git commit -m "inizio"_

_git remote remove origin_

_git remote add origin git@github.com:amunnezza/PythonCybersec.git_

_git branch -M main_

_git push -u origin main_

#### chiaramente potrebbe dare problemi se non hai la key registrata allora segui la procedura sul computer locale
ssh-keygen -o -t rsa -C "amunnezza@gmail.com"

#### crea una chiave pubblica e una privata nella directory .ssh partendo dalla home dell'utente
#### il contenuto della chiave pubblica (che un file nome.pub lo devi copiare sui settaggi dell'utente github che nel mio caso amunnezza andando in settings --> ssh and gpg keys -> premi il bottone New SSH key --> copia il contenuto del file.pub nella finestra e confermi)
#### aa questo punto il push dovrebbe funzionamere senza problemi






